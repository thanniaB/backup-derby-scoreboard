<script lang="js">
    import Counter from "./Counter.svelte";
    let { score } = $props();
</script>

<div>
    <input type="text" placeholder="Team Name" />
    <Counter count={score} />
</div>

<style>
    input,
    div {
        font-size: 6rem;
    }

    div {
        display: flex;
        flex-direction: column;
        align-items: center;
        overflow: hidden;
    }

    input {
        border: none;
        text-align: center;
    }
</style>