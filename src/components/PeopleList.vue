<template>
<h1>People list</h1>
<PeopleListItem />
<PeopleListItem />
<PeopleListItem />
</template>

<script>
import PeopleListItem from './PeopleListItem';
export default {
    name: 'PeopleList',
    components: {
        PeopleListItem,
    }

}
</script>