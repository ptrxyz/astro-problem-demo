<script>
    import { onMount } from 'svelte'

    let Carousel // for saving Carousel component class

    onMount(async () => {
        console.log('Seem this gets never executed ... ')
        const module = await import('svelte-carousel')
        Carousel = module.default
    })
</script>

<svelte:component this={Carousel}>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</svelte:component>
