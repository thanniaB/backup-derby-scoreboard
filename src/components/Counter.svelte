<script>
    let { count } = $props();

    function handleMinusOperator() {
        if (count > 0) {
            count --;
        }
    }
</script>

<div>
    <button onclick={() => handleMinusOperator()}>-</button>
    {count}
    <button onclick={() => count++}>+</button>
</div>

<style>
    div {
        display: flex;
    }

    button {
        background-color: white;
        border: none;
        font-size: 2rem;
    }
</style>
