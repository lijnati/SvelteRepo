<script>
  let count = 0;

  function Counter() {
    count+=0;
  }
</script>

<button on:click={Counter}>
Clicked {count} {count === 1 ? 'time' }
</button>