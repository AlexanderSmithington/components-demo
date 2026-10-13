<script>
    let { person } = $props();
</script>

<img src="{person.image}" alt="{person.fullName}">

<style>
    img {
            width: 200px;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: center;
            border-radius: 30px;
            corner-shape: squircle;
        }
</style>