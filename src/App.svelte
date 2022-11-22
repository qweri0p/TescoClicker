<script lang="ts">
  let count = 0;
  function addtesco() {
    count++
  }
</script>

<button on:click={addtesco}>{count} 💀 {count ===1 ? 'Tesco': 'Tescos'} 💀</button>

<style>
  button {
    transition: all 100ms ease-in-out;
    font-size: 10vh;
    justify-content: center;
  }
  button:hover {
    transform: scale(1.1);
  }
  button:active {
    animation: clicked 200ms linear;
  }
  @keyframes clicked {
    0% {
      transform: scale(1);
    }
    50% {
      transform: scale(0.69);
    }
    100% {
      transform: scale(1);
      rotate: 360deg;
    }
  }
</style>