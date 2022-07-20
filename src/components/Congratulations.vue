<template>
<h1 v-if="numberOfClicks >= 10">Congratulations! You've reached 10 clicks</h1>
</template>

<script>
export default {
    name: 'Congratulations',
    props: ['numberOfClicks'],
}

</script>