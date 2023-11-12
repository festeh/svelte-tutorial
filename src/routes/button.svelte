<script>
  function Increment() {
    count += 1;
  }
  let count = 0;
  $: double = count * 2;
  $: {
    console.log(`count is ${count}`);
    console.log(`double is ${double}`);
  }
  $: if (count >= 10) {
    alert(`count is dangerously high!`);
    count = 9;
  }
</script>

<button on:click={Increment}> 
Pressed {count} times
<br />
Double is {double}
</button>
