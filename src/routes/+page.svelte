<script>
    import Cloud from "$lib/components/cloud.svelte";
    let mode = "light";
    let switchModes = () => {
        if (mode == "light") mode = "dark";
        else if (mode == "dark") mode = "light";
        else throw Error("Unknown target state: " + mode);
    };
</script>

<Cloud top="" left="-5%" />

<main>
    <h1>{mode}</h1>
    <button on:click={switchModes}>Switch Modes</button>
</main>

<style>
    main {
        height: 100vh;
        margin: 0;
        text-align: center;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4rem;
        font-weight: 100;
        line-height: 1.1;
    }
</style>
