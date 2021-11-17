<script>
 export let value = 0;
 let digit=value;

 function increment() {
     digit = digit + 1;
 }
 function decrement() {
     digit = digit - 1;
 }
</script>

<svelte:options tag="c-ounter" />
<div class="counter">
    <button class="decrement" on:click={decrement}>-</button>
    <span class="digit">{digit}</span>
    <button class="increment" on:click={increment}>+</button>
</div>

<style>
 .counter {
     font-size: 1.5em;
     display: flex;
     margin: 0.5em;
 }
 button {
     border: 0;
     width: 60px;
     height: 50px;
     margin: 5px;
     font-size: 20px;
 }
 button.decrement {
     background-color: #ffadad;
 }
 button.increment {
     background-color: #a0c4ff;
 }

 .digit {
     display: flex;
     align-items: center;
     padding-left: 0.5em;
     padding-right: 0.5em;
 }
</style>
