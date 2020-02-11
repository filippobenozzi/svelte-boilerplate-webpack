<script>
  import { Router, Route } from 'svelte-routing'
  import { Layout, NavLink } from '@components'
  import Home from '@views/Home'
  import Hello from '@views/Hello'
  import Something from '@views/Something'

  export let url = ''
</script>

<Router {url}>
  <nav>
    <NavLink to="/">Home</NavLink>
    <NavLink to="hello">Hello</NavLink>
    <NavLink to="something">Something</NavLink>
  </nav>
  <div>
    <Layout path="/" title="" component={Home} />
    <Layout path="hello" title="Hello" component={Hello} />
    <Layout path="something" title="Something" component={Something} />
  </div>
</Router>
