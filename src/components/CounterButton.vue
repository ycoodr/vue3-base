<template>
<p>You have clicked the button {{ numberOfClicks }} times</p>
<button @click="$emit('increment')" >Click me!</button>
</template>

<script>
export default {
    name: 'CounterButton',
    props: ['numberOfClicks'],
    
}
</script>