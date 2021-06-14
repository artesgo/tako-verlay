<script lang="ts">
	import Bottom from './lib/Bottom.svelte';
import Left from './lib/Left.svelte';
import Right from './lib/Right.svelte';
import Top from './lib/Top.svelte';
</script>

<main>
  <div class="top flex around">
    <Top></Top>
  </div>
  <div class="middle flex between">
    <div class="left">
      <Left></Left>
    </div>
    <div class="right">
      <Right></Right>
    </div>
  </div>
  <div class="bottom flex around">
    <Bottom></Bottom>
  </div>
</main>

<style global>
  body {
    background: green;
    padding: 0;
    margin: 0;
  }

  main {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100vh;
  }
  .flex {
    display: flex;
  }
  .between {
    justify-content: space-between; 
  }
  .around {
    justify-content: space-around; 
  }
</style>