<script>
    import JamNumber from "../components/JamNumber.svelte";
    import TeamScore from "../components/TeamScore.svelte";
	let team1score = $state(0);
    let team2score = $state(0);
    let jamNumber = $state(1);
</script>

<main>
    <TeamScore score={team1score} />
    <JamNumber jamNumber={jamNumber} />
    <TeamScore score={team2score} />
</main>

<style>
    main {
        display: grid;
        align-items: center;
        grid-template-columns: 40% auto 40%;
        height: 100vh;
        font-family: 'Trebuchet MS', sans-serif;
    }
</style>