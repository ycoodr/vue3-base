<template>
<LifeCycleTest v-if="numberOfClicks < 10" :numberOfClicks="numberOfClicks"/>
<Congratulations :numberOfClicks="numberOfClicks" />
<CounterButton @increment="increment" :numberOfClicks="numberOfClicks" />
<PeopleList />
</template>

<script>
import PeopleList from './components/PeopleList';
import CounterButton from './components/CounterButton';
import Congratulations from './components/Congratulations';
import LifeCycleTest from './components/LifeCycleTest';

export default {
  name: 'App',
  components: {
    PeopleList,
    CounterButton,
    Congratulations,
    LifeCycleTest,
  },

  data(){
        return {
            numberOfClicks: 0,
        };
    },
    methods: {
        increment() {
            this.numberOfClicks += 1;
        }
    }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
