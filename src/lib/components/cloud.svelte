<script>
    import cloud from "$lib/assets/cloud.svg";

    export let top = 0;
    export let left = 0;
    $: cssVarStyles = `left:${left}; top:${top};`;
</script>

<img class="cloud" src={cloud} alt="cloud" style={cssVarStyles} />

<style>
    .cloud {
        position: absolute;
        width: 20vw;
        height: auto;
        min-width: 100px;
        max-width: 300px;
    }
</style>
