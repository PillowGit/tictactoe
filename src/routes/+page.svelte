<script lang="ts">
  let roomcode: string = "abc123";
</script>

<div class="main-page-content">
  <h1 class="title">
    <span id="a">Tic </span>
    <span id="b"> Tac </span>
    <span id="c"> Toe</span>
  </h1>
  <div class="options">
    <button class="newroom">New Room</button>
    <div class="seperator"></div>
    <div class="roominput">
      <span class="roominputprompt">Enter Room Code:</span>
      <div class="roomcode">
        <input
          type="text"
          placeholder="#abc123"
          bind:value={roomcode}
          class="roomcodefield"
        />
        <img
          src="icons/right-arrow.svg"
          alt="submit"
          class="roomcodesubmit"
          on:click={() => alert("Room code: " + roomcode)}
          on:keydown={(e) => {
            if (e.key === "Enter") {
              alert("Room code: " + roomcode);
            }
          }}
          role="button"
          tabindex="0"
          aria-pressed="false"
        />
      </div>
    </div>
  </div>
</div>

<style>
  .roominput {
    width: 10%;
    height: 90%;
    font-size: 1vw;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .roomcode {
    height: 80%;
    display: flex;
    justify-content: space-between;
  }
  .roominputprompt {
    height: 40%;
    font-size: 1.1vw;
  }
  .roomcodefield {
    font-size: 1.8vw;
    width: 70%;
    height: 60%;
    background: none;
    color: var(--text-color);
    border: none;
    border-bottom: 0.15vw solid
      color-mix(in srgb, var(--text-color) 50%, transparent);
    align-self: center;
  }
  .roomcodesubmit {
    aspect-ratio: 1 / 1;
    height: 2vw;
    align-self: center;
    margin: none;
    padding: none;
    -webkit-filter: invert(0.8);
    filter: invert(0.8);
    transition: 0.2s;
  }
  .roomcodesubmit:hover {
    transform: scale(1.1);
    -webkit-filter: invert(0.6);
    filter: invert(0.6);
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
    height: 10vh;
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
    animation: exist 0.75s ease-in-out forwards;
    animation-delay: 1s;
  }
  #b {
    opacity: 0;
    animation: exist 0.75s ease-in-out forwards;
    animation-delay: 1.75s;
  }
  #c {
    opacity: 0;
    animation: exist 0.75s ease-in-out forwards;
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
