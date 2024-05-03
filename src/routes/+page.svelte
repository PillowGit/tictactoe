<script lang="ts">
  let roomcode: string = '';
</script>

<div class="main-page-content">
  <h1 class="title"><span id="a">Svelte</span><span id="b">Kit</span><span id="c">!</span></h1>
  <div class="options">
    <button class="newroom">New Room</button>
    <div class="seperator"></div>
    <div class="roominput">
      <span>Enter Room Code:</span>
      <input type="text" placeholder="#abc123" bind:value={roomcode} class="roomcode" />
      <button>-></button>
    </div>
  </div>
</div>

<style>
  .roominput {
    width: 10%;
    height: 90%;
    font-size: 1vw;
    display: flex;
    flex-flow: column nowrap;
    align-items: flex-start;
    justify-content: space-between;
    border: 1px solid red;
  }
  .roomcode {
    font-size: 1.8vw;
    width: 95%;
    height: 30%;
    background: none;
    color: var(--text-color);
    border: none;
    border-bottom: 0.15vw solid color-mix(in srgb, var(--text-color) 50%, transparent);
  }

  .title {
    width: 70%;
    text-align: center;
  }
  .main-page-content {
    height: 100vh;
    width: 100vw;
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: 2.75vw;
  }
  .options {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    min-height: 10vh;
  }
  .seperator {
    margin-left: 2%;
    margin-right: 2%;
    height: 75%;
    background-color: color-mix(in srgb, var(--text-color) 50%, transparent);
    width: 0.05%;
  }
  .newroom {
    width: 10%;
    height: 65%;
    font-size: 1.25vw;
    color: var(--text-color);
    background: none;
    cursor: pointer;
    border: 0.15vw solid color-mix(in srgb, var(--text-color) 50%, transparent);
    border-radius: 1vw;
    --webkit-backdrop-filter: blur(0.5vw);
    backdrop-filter: blur(0.5vw);
    transition: 0.2s;
  }
  .newroom:hover {
    background-color: color-mix(in srgb, var(--text-color) 10%, transparent);
    transform: scale(1.03);
  }
  #a {
    opacity: 0;
    animation: exist .75s ease-in-out forwards;
    animation-delay: 1s;
  }
  #b {
    opacity: 0;
    animation: exist .75s ease-in-out forwards;
    animation-delay: 1.75s;
  }
  #c {
    opacity: 0;
    animation: exist .75s ease-in-out forwards;
    animation-delay: 2.5s;
  }
  @keyframes exist {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
      transform: none;
    }
  }
</style>