<template>
    <section>
        <h1>{{pageTitle}}</h1>
        <h4>Users:</h4> 
        <ul>
            <li v-for="user of users" :key="user.id">
                <a href="#" @click.prevent="openUser(user)"> {{user.name}} </a>
            </li>
        </ul>
    </section>
</template>

<script>
export default {
    async fetch({store}) {
  if (store.getters['users/users'].length === 0) {
      await store.dispatch('users/fetch')
  }
    },
    // async asyncData({$axios}) {
    //    const users = await $axios.$get('http://jsonplaceholder.typicode.com/users')
    //    return {users}
    // },
    data: () =>({
        pageTitle: 'About'
    }),
    computed: {
        users() {
            return this.$store.getters['users/users']
        }
    },
   //async mounted() {
   //  this.users = await this.$axios.$get('http://jsonplaceholder.typicode.com/users')
   //},
    methods: {
        openUser(user) {
            this.$router.push('/about/' + user.id)
        }
        },
        layout: 'empty'
}
</script>

<style scoped>

h1{
    color: blue;
    font-size: 34px;
    padding-top: 20px ;
    padding-right: 100px;
}

h4{
    color: rgb(1, 1, 114);
    font-size: 30px;
    padding-top: 40px ;
    padding-left: 12px;
    padding-bottom: 30px;
}

li {
 padding-right: 82px;
 text-decoration: none;
   list-style: none;
    font-family: helvetica, arial, sans-serif;
    font-size: 24px;
    line-height: 2;
    color: rgb(3, 7, 44);
}

</style>