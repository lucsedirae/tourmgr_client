<script>
  import { Router, Link, Route } from 'svelte-routing';

  import About from './core/components/layout/About.svelte';
	import Login from './core/components/user/Login.svelte'
  import Navbar from './core/components/layout/Navbar.svelte';
  import Register from './core/components/user/Register.svelte';

  export let url = '';
</script>

<Router {url}>
  <main>
    <Navbar />
		<div>
			<Route path="register" component={Register} />
			<Route path="login" component={Login} />
			<Route path="/"><About /></Route>
		</div>
	</main>
</Router>
