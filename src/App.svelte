<script lang="ts">
  import Router from 'svelte-spa-router';
  import Home from './Home.svelte';
  import Layout from './Layout.svelte';
import Nav from './Nav.svelte';
  import UtilCalculator from './UtilCalculator.svelte';

  const routes = {
    '/': Home,
    '/util-calculator': UtilCalculator,
  }
</script>

<Layout>
  <Nav />
  <Router {routes} />
</Layout>
