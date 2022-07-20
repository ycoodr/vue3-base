<template>
<h1>I'm the timer</h1>
</template>

<script>
export default {
    name: 'Timer',
    props: ['delay', 'name'],
    created(){
        setInterval(() => {
            this.$emit('tick', this.name);
        }, this.delay);
    }
}
</script>