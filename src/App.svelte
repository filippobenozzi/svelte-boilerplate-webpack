<script>
  import { Router, Link, Route } from 'svelte-routing'
  import Home from '@views/Home'
  import Hello from '@views/Hello'
  import Something from '@views/Something'

  export let url = ''
</script>

<Router {url}>
  <nav>
    <Link to="/">Home</Link>
    <Link to="hello">Hello</Link>
    <Link to="something">Something</Link>
  </nav>
  <div>
    <Route path="/" component={Home} />
    <Route path="hello" component={Hello} />
    <Route path="something" component={Something} />
  </div>
</Router>
