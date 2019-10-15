<template>
    <gyatso v-slot:header="{user}">
    <h2>this is the header blog</h2>
    <ul>
    <li v-for="user in user">
    {{user.name}}
    {{user.age}}
    </li>
    </ul>
    <h3> king is never back down</h3>
    </gyatso>
</template>

<script>
import Gyatso from './Gyatso.vue';

export default {
    components: {
    'gyatso':Gyatso
    },
    data () {
        return {
        }
    },
    methods: {
    }
}
</script>

<style scoped>

</style>
