<script>
    import Card from '$lib/components/Card.svelte';
    let persons = [
        {
            fullName: "Phill Connors",
            favSong: "I Got You Babe",
            petName: "Punxsutawney Phil"
        },
        {
            fullName: "Bhill Monnors",
            favSong: "Australian National Anthem",
            petName: "FinkleTingly Phil"
        },
        {
            fullName: "Joe Bingle",
            favSong: "Nothing, He hates music",
            petName: "Punxsutawney Phil"
        },
    ];
</script>

<main>
<!-- Make loop -->
{#each persons as person}
    <Card person={person} />  
{/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>