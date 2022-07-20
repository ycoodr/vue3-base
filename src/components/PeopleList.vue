<template>
<h1>People list</h1>
<PeopleListItem :person="person1" />
<PeopleListItem :person="person2" />
<PeopleListItem :person="person3" />
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
            person1: { name: 'Shaun', age: 100, hairColor: 'brown'},
            person2: { name: 'John', age: 50, hairColor: 'green' },
            person3: { name: 'Nancy', age: 34, hairColor: 'red' } ,
        }
    }
    

}
</script>