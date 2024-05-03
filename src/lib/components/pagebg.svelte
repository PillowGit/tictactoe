<div class="area">
  <ul class="bottom-dots">
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
  </ul>
  <ul class="top-dots">
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
    <li class="dot"></li>
  </ul>
</div>

<style>
  /* Define the drawn area */
  .area {
    position: fixed;
    z-index: -15;
    left: 0;
    top: 0;
    height: 100vh;
    width: 100vw;
    background-color: #37393A;
  }
  /* Create variables for top and bottom curves */
  .bottom-dots {
    --start: #6A66A3;
    --end: #B3CBB9;
  }
  .top-dots {
    --start: #EDAE49;
    --end: #A9DDD6;
  }
  /* Create offsets for animations */
  .bottom-dots li:nth-child(1) {
    --x-off: 0vw;
    --y-off: 0vh;
    --duration: 9s;
  }
  .bottom-dots li:nth-child(2) {
    --x-off: -12vw;
    --y-off: -2vh;
    --duration: 13s;
  }
  .bottom-dots li:nth-child(3) {
    --x-off: -3vw;
    --y-off: -4vh;
    --duration: 17s;
  }
  .bottom-dots li:nth-child(4) {
    --x-off: -23vw;
    --y-off: -10vh;
    --duration: 28s;
  }
  .bottom-dots li:nth-child(5) {
    --x-off: -29vw;
    --y-off: -1vh;
    --duration: 17s;
  }
  .bottom-dots li:nth-child(6) {
    --x-off: 0vw;
    --y-off: 0vh;
    --duration: 39s;
  }
  .bottom-dots li:nth-child(7) {
    --x-off: -9vw;
    --y-off: -18vh;
    --duration: 20s;
  }
  .bottom-dots li:nth-child(8) {
    --x-off: -10vw;
    --y-off: -8vh;
    --duration: 16s;
  }
  .bottom-dots li:nth-child(9) {
    --x-off: -30vw;
    --y-off: 0vh;
    --duration: 40s;
  }
  .bottom-dots li:nth-child(10) {
    --x-off: 0vw;
    --y-off: -20vh;
    --duration: 20s;
  }
  .bottom-dots li:nth-child(11) {
    --x-off: -10vw;
    --y-off: -30vh;
    --duration: 40s;
  }
  .bottom-dots li:nth-child(12) {
    --x-off: 0vw;
    --y-off: -40vh;
    --duration: 20s;
  }
  .bottom-dots li:nth-child(13) {
    --x-off: -10vw;
    --y-off: -5vh;
    --duration: 25s;
  }
  .bottom-dots li:nth-child(14) {
    --x-off: -2vw;
    --y-off: -10vh;
    --duration: 15s;
  }
  .bottom-dots li:nth-child(15) {
    --x-off: -18vw;
    --y-off: -20vh;
    --duration: 25s;
  }
  .bottom-dots li:nth-child(16) {
    --x-off: 0vw;
    --y-off: -30vh;
    --duration: 15s;
  }
  .top-dots li:nth-child(1) {
    --x-off: 0vw;
    --y-off: 0vh;
    --duration: 9s;
  }
  .top-dots li:nth-child(2) {
    --x-off: 12vw;
    --y-off: -2vh;
    --duration: 13s;
  }
  /* Make offsets and durations random */
  .top-dots li:nth-child(3) {
    --x-off: 3vw;
    --y-off: -4vh;
    --duration: 17s;
  }
  .top-dots li:nth-child(4) {
    --x-off: 23vw;
    --y-off: -10vh;
    --duration: 28s;
  }
  .top-dots li:nth-child(5) {
    --x-off: 29vw;
    --y-off: -1vh;
    --duration: 17s;
  }
  .top-dots li:nth-child(6) {
    --x-off: 0vw;
    --y-off: 0vh;
    --duration: 39s;
  }
  .top-dots li:nth-child(7) {
    --x-off: 9vw;
    --y-off: -18vh;
    --duration: 20s;
  }
  .top-dots li:nth-child(8) {
    --x-off: 10vw;
    --y-off: -8vh;
    --duration: 16s;
  }
  .top-dots li:nth-child(9) {
    --x-off: 30vw;
    --y-off: 0vh;
    --duration: 37s;
  }
  .top-dots li:nth-child(10) {
    --x-off: 0vw;
    --y-off: -20vh;
    --duration: 20s;
  }
  .top-dots li:nth-child(11) {
    --x-off: 10vw;
    --y-off: -30vh;
    --duration: 33s;
  }
  .top-dots li:nth-child(12) {
    --x-off: 0vw;
    --y-off: -40vh;
    --duration: 28s;
  }
  .top-dots li:nth-child(13) {
    --x-off: 10vw;
    --y-off: -5vh;
    --duration: 25s;
  }
  .top-dots li:nth-child(14) {
    --x-off: 2vw;
    --y-off: -10vh;
    --duration: 15s;
  }
  .top-dots li:nth-child(15) {
    --x-off: 18vw;
    --y-off: -20vh;
    --duration: 25s;
  }
  .top-dots li:nth-child(16) {
    --x-off: 0vw;
    --y-off: -30vh;
    --duration: 15s;
  }
  .dot {
    height: 3vh;
    width: 3vh;
    top: -3vh;
    left: -3vw;
    background-color: var(--start);
    border-radius: 50%;
    display: inline-block;
    position: absolute;
    opacity: 45%;
  }
  .bottom-dots .dot {
    top: 150vh;
    left: -3vw;
    animation: bottom-curve var(--duration) linear infinite;
  }
  .top-dots .dot {
    animation: top-curve var(--duration) linear infinite;
  }
  @keyframes bottom-curve {
    0% {
      top: calc(50vh - 50vh * (1 / -5) + var(--y-off));
      left: calc(50vw + 1vw * (-5 * 10) + var(--x-off));
    }
    5% {
      top: calc(50vh - 50vh * (1 / -4.75) + var(--y-off));
      left: calc(50vw + 1vw * (-4.75 * 10) + var(--x-off));
    }
    10% {
      top: calc(50vh - 50vh * (1 / -4.5) + var(--y-off));
      left: calc(50vw + 1vw * (-4.5 * 10) + var(--x-off));
    }
    15% {
      top: calc(50vh - 50vh * (1 / -4.25) + var(--y-off));
      left: calc(50vw + 1vw * (-4.25 * 10) + var(--x-off));
    }
    20% {
      top: calc(50vh - 50vh * (1 / -4) + var(--y-off));
      left: calc(50vw + 1vw * (-4 * 10) + var(--x-off));
    }
    25% {
      top: calc(50vh - 50vh * (1 / -3.75) + var(--y-off));
      left: calc(50vw + 1vw * (-3.75 * 10) + var(--x-off));
    }
    30% {
      top: calc(50vh - 50vh * (1 / -3.5) + var(--y-off));
      left: calc(50vw + 1vw * (-3.5 * 10) + var(--x-off));
    }
    35% {
      top: calc(50vh - 50vh * (1 / -3.25) + var(--y-off));
      left: calc(50vw + 1vw * (-3.25 * 10) + var(--x-off));
    }
    40% {
      top: calc(50vh - 50vh * (1 / -3) + var(--y-off));
      left: calc(50vw + 1vw * (-3 * 10) + var(--x-off));
    }
    45% {
      top: calc(50vh - 50vh * (1 / -2.75) + var(--y-off));
      left: calc(50vw + 1vw * (-2.75 * 10) + var(--x-off));
    }
    50% {
      top: calc(50vh - 50vh * (1 / -2.5) + var(--y-off));
      left: calc(50vw + 1vw * (-2.5 * 10) + var(--x-off));
    }
    55% {
      top: calc(50vh - 50vh * (1 / -2.25) + var(--y-off));
      left: calc(50vw + 1vw * (-2.25 * 10) + var(--x-off));
    }
    60% {
      top: calc(50vh - 50vh * (1 / -2) + var(--y-off));
      left: calc(50vw + 1vw * (-2 * 10) + var(--x-off));
    }
    65% {
      top: calc(50vh - 50vh * (1 / -1.75) + var(--y-off));
      left: calc(50vw + 1vw * (-1.75 * 10) + var(--x-off));
    }
    70% {
      top: calc(50vh - 50vh * (1 / -1.5) + var(--y-off));
      left: calc(50vw + 1vw * (-1.5 * 10) + var(--x-off));
    }
    75% {
      top: calc(50vh - 50vh * (1 / -1.25) + var(--y-off));
      left: calc(50vw + 1vw * (-1.25 * 10) + var(--x-off));
    }
    80% {
      top: calc(50vh - 50vh * (1 / -1) + var(--y-off));
      left: calc(50vw + 1vw * (-1 * 10) + var(--x-off));
    }
    85% {
      top: calc(50vh - 50vh * (1 / -0.75) + var(--y-off));
      left: calc(50vw + 1vw * (-0.75 * 10) + var(--x-off));
    }
    90% {
      top: calc(50vh - 50vh * (1 / -0.5) + var(--y-off));
      left: calc(50vw + 1vw * (-0.5 * 10) + var(--x-off));
    }
    95% {
      top: calc(50vh - 50vh * (1 / -0.25) + var(--y-off));
      left: calc(50vw + 1vw * (-0.25 * 10) + var(--x-off));
    }
    100% {
      top: calc(100vh + var(--y-off)); 
      left: calc(50vw + var(--x-off));
      background-color: var(--end); 
      opacity: 0;
    }
  }
  @keyframes top-curve {
    0% {
      top: calc(50vh - 50vh * (1 / 5) + var(--y-off)); 
      left: calc(50vw + 1vw * (5 * 10) + var(--x-off)); 
    }
    5% {
      top: calc(50vh - 50vh * (1 / 4.75) + var(--y-off)); 
      left: calc(50vw + 1vw * (4.75 * 10) + var(--x-off));
    }
    10% {
      top: calc(50vh - 50vh * (1 / 4.5) + var(--y-off)); 
      left: calc(50vw + 1vw * (4.5 * 10) + var(--x-off));
    }
    15% {
      top: calc(50vh - 50vh * (1 / 4.25) + var(--y-off)); 
      left: calc(50vw + 1vw * (4.25 * 10) + var(--x-off));
    }
    20% {
      top: calc(50vh - 50vh * (1 / 4) + var(--y-off)); 
      left: calc(50vw + 1vw * (4 * 10) + var(--x-off));
    }
    25% {
      top: calc(50vh - 50vh * (1 / 3.75) + var(--y-off)); 
      left: calc(50vw + 1vw * (3.75 * 10) + var(--x-off));
    }
    30% {
      top: calc(50vh - 50vh * (1 / 3.5) + var(--y-off)); 
      left: calc(50vw + 1vw * (3.5 * 10) + var(--x-off));
    }
    35% {
      top: calc(50vh - 50vh * (1 / 3.25) + var(--y-off)); 
      left: calc(50vw + 1vw * (3.25 * 10) + var(--x-off));
    }
    40% {
      top: calc(50vh - 50vh * (1 / 3) + var(--y-off)); 
      left: calc(50vw + 1vw * (3 * 10) + var(--x-off));
    }
    45% {
      top: calc(50vh - 50vh * (1 / 2.75) + var(--y-off)); 
      left: calc(50vw + 1vw * (2.75 * 10) + var(--x-off));
    }
    50% {
      top: calc(50vh - 50vh * (1 / 2.5) + var(--y-off)); 
      left: calc(50vw + 1vw * (2.5 * 10) + var(--x-off));
    }
    55% {
      top: calc(50vh - 50vh * (1 / 2.25) + var(--y-off)); 
      left: calc(50vw + 1vw * (2.25 * 10) + var(--x-off));
    }
    60% {
      top: calc(50vh - 50vh * (1 / 2) + var(--y-off)); 
      left: calc(50vw + 1vw * (2 * 10) + var(--x-off));
    }
    65% {
      top: calc(50vh - 50vh * (1 / 1.75) + var(--y-off)); 
      left: calc(50vw + 1vw * (1.75 * 10) + var(--x-off));
    }
    70% {
      top: calc(50vh - 50vh * (1 / 1.5) + var(--y-off)); 
      left: calc(50vw + 1vw * (1.5 * 10) + var(--x-off));
    }
    75% {
      top: calc(50vh - 50vh * (1 / 1.25) + var(--y-off)); 
      left: calc(50vw + 1vw * (1.25 * 10) + var(--x-off));
    }
    80% {
      top: calc(50vh - 50vh * (1 / 1) + var(--y-off)); 
      left: calc(50vw + 1vw * (1 * 10) + var(--x-off));
    }
    85% {
      top: calc(50vh - 50vh * (1 / 0.75) + var(--y-off)); 
      left: calc(50vw + 1vw * (0.75 * 10) + var(--x-off));
    }
    90% {
      top: calc(50vh - 50vh * (1 / 0.5) + var(--y-off)); 
      left: calc(50vw + 1vw * (0.5 * 10) + var(--x-off));
    }
    95% {
      top: calc(50vh - 50vh * (1 / 0.25) + var(--y-off)); 
      left: calc(50vw + 1vw * (0.25 * 10) + var(--x-off));
    }
    100% {
      top: calc(-100vh + var(--y-off)); 
      left: calc(50vw + var(--x-off));
      background-color: var(--end); 
      opacity: 0;
    }
  }
</style>
