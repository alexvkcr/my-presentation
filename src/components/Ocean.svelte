<script></script>

<div class="ocean">
  <svg
    class="editorial"
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
    viewBox="0 24 150 28"
    preserveAspectRatio="none"
  >
    <defs>
      <path
        id="gentle-wave"
        d="M-160 44c30 0 
            58-18 88-18s
            58 18 88 18 
            58-18 88-18 
            58 18 88 18
            v44h-352z"
      />
    </defs>
    <g class="parallax">
      <use xlink:href="#gentle-wave" x="50" y="0" fill="#4579e2" />
      <use xlink:href="#gentle-wave" x="50" y="3" fill="#3461c1" />
      <use xlink:href="#gentle-wave" x="50" y="6" fill="#2d55aa" />
    </g>
  </svg>
  <div class="content">
    <h1 contenteditable="true" />
  </div>
</div>

<style>
  ::selection {
    background-color: salmon;
    color: white;
  }
  .parallax > use {
    animation: move-forever 52s linear infinite;
  }
  .parallax > use:nth-child(1) {
    animation-delay: -2s;
  }
  .parallax > use:nth-child(2) {
    animation-delay: -2s;
    animation-duration: 25s;
  }
  .parallax > use:nth-child(3) {
    animation-delay: -4s;
    animation-duration: 13s;
  }
  @keyframes move-forever {
    0% {
      transform: translate(-90px, 0%);
    }
    100% {
      transform: translate(85px, 0%);
    }
  }
  .editorial {
    display: block;
    width: 100%;
    height: 10em;
    max-height: 100vh;
    margin: 0;
  }
  .ocean {
    z-index: 1;
    margin: 0;
    max-height: 30vh;
    overflow: hidden;
    padding: 57.3vh 0 0 0;
  }
  .content {
    font-family: "Lato", sans-serif;
    text-align: center;
    background-color: #2d55aa;
    text-align: center;
    min-height: 75vh;
    margin: -0.1em 0 0 0;
    color: #eee;
    font-size: 2em;
    font-weight: 300;
  }
  .content {
    font-size: 1em;
  }
  .content h1 {
    margin-top: -1.3em;
    font-weight: 100;
    font-size: 5em;
    user-select: none;
    cursor: default;
  }
  /*prevent many large-by-comparison ripples by shrinking the height*/
  @media (max-width: 50em) {
    .content h1 {
      font-size: 12vmax;
    }
    .editorial {
      height: 17vw;
    }
  }
  h1 {
    outline: none;
  }
</style>
