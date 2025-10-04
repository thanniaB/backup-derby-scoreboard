<script lang="js">
    import Counter from "./Counter.svelte";
    let { jamNumber } = $props();
</script>

<div>
    <div>Jam</div>
    <Counter count={jamNumber} />
</div>

<style>
    div {
        display: flex;
        flex-direction: column;
        align-items: center;
        font-size: 4rem;
    }
</style>