<script>
  
  let name = 'Ivy';
  let count = 0;
  

  function handleClick() {
    count += 1;
  }
</script>


{#if name === 'Ivy'}
  <h1>Hello {name}!</h1>
{:else}
  <h1>I don't say hello to anyone else</h1>
{/if}

<button on:click={handleClick}>
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>

<input bind:value={name} placeholder="Enter your name" />
<p>Happy Halloween {name}!</p>
