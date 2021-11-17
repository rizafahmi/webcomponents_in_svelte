<script>
import './Counter.svelte'
</script>

<svelte:options tag="web-components" />
<main>
    <h1>Counter</h1>
    <c-ounter />
</main>

<style>
    main {
        display: grid;
        place-items: center;
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
