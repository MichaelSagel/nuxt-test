<template>

    <div>

        <h1>Users page</h1>

        <hr>

        <ul>

            <li v-for="user in users" :key="user.id">

                {{user.name}}

            </li>

        </ul>

    </div>

</template>

<script>
export default {

    async asyncData() {

        const response = await fetch('https://jsonplaceholder.typicode.com/users?_limit=5')
        const users = await response.json()
        return {users}
    },

    data: () => ({
        users: []
    }),

    async mounted() {

    }
    
}
</script>

<style  scoped>

    hr {

        margin-top: 20px;
        margin-bottom: 20px;

    }

</style>