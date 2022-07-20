<template>
<div>
<h3>{{ name }}</h3>
<p>Age: {{ age }} years</p>
<p>Hair color: {{ hairColor }}</p>
</div>
</template>

<script>
export default {
    name: 'PeopleListItem',
    data(){
        return {
            name: 'Shaun Wassel',
            age: 100,
            hairColor: 'brown',
        }
    }
}
</script>