<script>
    import Card from '$lib/components/Card.svelte';
    import billm1 from '$lib/assets/images/groundhog-day.webp';
    import billm2 from '$lib/assets/images/bill-murray-at-the-29th-annual-screen-actors-guild-awards-news-photo-1693940600.webp';
    import billm3 from '$lib/assets/images/images.webp';
    let persons = [
        {
            fullName: "Phill Connors",
            favSong: "I Got You Babe",
            petName: "Punxsutawney Phil",
            image: billm1
        },
        {
            fullName: "Bhill Monnors",
            favSong: "Australian National Anthem",
            petName: "FinkleTingly Phil",
            image: billm2
        },
        {
            fullName: "Joe Bingle",
            favSong: "Nothing, He hates music",
            petName: "Punxsutawney Phil",
            image: billm3
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