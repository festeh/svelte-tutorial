<script>
  import Nested from "./nested.svelte";
  import Button from "./button.svelte";
  var name = "Dima";
  // upercase name
  $: name = name.toUpperCase();
  // image of a nice cat
  let src = "https://placekitten.com/200/300";
</script>

<h1>Hello {name}</h1>
<p>How are you?</p>
<Nested />
<img {src} alt="" />
<Button />

<style>
  h1 {
    color: red;
  }
  p {
    color: blue;
    text-align: center;
    font-size: 40px;
  }
</style>
