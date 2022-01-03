<script>
  import Layout from './core/components/layout/Layout.svelte';
	import Home from './core/components/pages/Home.svelte'
	import Register from './core/components/pages/Register.svelte'
  import { Router, Link, Route } from 'svelte-routing';
  export let url = '';
</script>

<Router {url}>
  <nav>
    <Link to="/" class='link light'>Home</Link>
		<Link to='register' class='link light'>Register</Link>
  </nav>
  <div>
		<Route path='register' component={Register}/>
    <Route path="/"><Home /></Route>
  </div>
</Router>
