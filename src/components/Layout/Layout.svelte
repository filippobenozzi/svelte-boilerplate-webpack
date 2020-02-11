<script>

    import { Route } from 'svelte-routing'
    import { Head } from '@components'

    export let path = ''
    export let component = null
    export let title = ''

</script>

<Route path="{path}">
    <Head title="{title}" />
    <main>
        <svelte:component this="{component}"  />
    </main>
</Route>
