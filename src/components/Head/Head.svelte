<script>

    import 'bulma/css/bulma.min.css'

    export let title
    const base_title = 'Svelte App'

</script>

<svelte:head>

    {#if title}
        <title>{title} - {base_title}</title>
    {:else}
        <title>{base_title}</title>
    {/if}

</svelte:head>
