<template>
<h1>This is a lifecycle test</h1>
</template>

<script>
export default {
    name: 'LifeCycleTest',
    props: ['numberOfClicks'],
    beforeCreate(){
        console.log('in beforeCreate');
    },
    created(){
        console.log('in created');
    },
    beforeMount(){
        console.log('in beforeMounted');
    },
    mounted(){
        console.log('in mounted');
    },
    beforeUpdate(){
        console.log('in beforeUpdate');
    },
    updated(){
        console.log('in updated');
    },
    beforeUnmount(){
        console.log('in beforeUnmount');
    },
    unmounted(){
        console.log('in unmounted');
    },
}
</script>