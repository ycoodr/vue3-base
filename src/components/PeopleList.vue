<template>
<h1>People list</h1>
<PeopleListItem v-for="person in people" :key="person.name" :person="person" />

</template>

<script>
import PeopleListItem from './PeopleListItem';
export default {
    name: 'PeopleList',
    components: {
        PeopleListItem,
    },
    data(){
        return {
            people: [
             { name: 'Shaun', age: 100, hairColor: 'brown'},
             { name: 'John', age: 50, hairColor: 'green' },
             { name: 'Nancy', age: 34, hairColor: 'red' } ,
            ],

           
        }
    }
    

}
</script>

<style scoped>
h1 {
    color: red;
}
</style>