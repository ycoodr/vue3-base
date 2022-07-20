<template>
<!-- <LifeCycleTest v-if="numberOfClicks < 10" :numberOfClicks="numberOfClicks"/>
<Congratulations :numberOfClicks="numberOfClicks" />
<CounterButton @increment="increment" :numberOfClicks="numberOfClicks" />
<Timer @tick="onTick" name="Timer 1"  :delay="2000" />
<Timer @tick="onTick" name="Timer 2" :delay="5000" />-->
<h1>My vue app</h1>
<PeopleList /> 
<!-- <FlashingMessage message="Hello friends!" :delay="500" /> -->
</template>

<script>
import PeopleList from './components/PeopleList';
// import CounterButton from './components/CounterButton';
// import Congratulations from './components/Congratulations';
// import LifeCycleTest from './components/LifeCycleTest';
// import Timer from './components/Timer';
// import FlashingMessage from './components/FlashingMessage';

export default {
  name: 'App',
  components: {
    PeopleList,
    // CounterButton,
    // Congratulations,
    // LifeCycleTest,
    // Timer,
    // FlashingMessage,
  },

  data(){
        return {
            numberOfClicks: 0,
        };
    },
    methods: {
        increment() {
            this.numberOfClicks += 1;
        },
        onTick(name){
          console.log(name + ': Tick!');
        }
    }
}
</script>

<style scoped>
h1 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
