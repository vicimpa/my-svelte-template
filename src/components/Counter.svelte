<script lang="ts">
  export let counter = 0;

  const inc = () => counter++;
  const dec = () => counter--;
  const res = () => (counter = 0);
</script>

<div class="counter">
  <div>Counter {counter}</div>
  <div>
    <button on:click={inc}>+</button>
    <button on:click={dec}>-</button>
    <button on:click={res}>C</button>
  </div>
</div>

<style lang="sass">
  .counter
    display: flex
    flex-direction: column
    border: 1px solid #999
    padding: 10px
    gap: 10px

    button
      padding: 5px 10px
      cursor: pointer
</style>
