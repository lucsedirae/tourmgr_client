<script>
  // Data
  import { siteName } from './config/site/siteconfig.json';
  import { str_home, str_register, str_login } from './config/lang/lang.json';

  // Components
  import Home from './core/components/pages/Home.svelte';
  import Login from './core/components/pages/Login.svelte';
  import Register from './core/components/pages/Register.svelte';
  import { Router, Link, Route } from 'svelte-routing';
  export let url = '';
</script>

<Router {url}>
  <nav>
    <h1 class=" brand">{siteName}</h1>
    <Link to="/" class="link light">{str_home}</Link>
    <Link to="register" class="link light">{str_register}</Link>
    <Link to="login" class="link light">{str_login}</Link>
  </nav>
  <div>
    <Route path="register" component={Register} />
    <Route path="login" component={Login} />
    <Route path="/"><Home /></Route>
  </div>
</Router>
