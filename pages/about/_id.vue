<template>
    <section>
        <h1>{{user.name}} </h1>
        <h3>{{user.email}}</h3>
        <h4>city: {{user.address.city}}</h4> 

        <li> 
            <a href="/about">About Page</a>
        </li>
    </section>
</template>

<script>
export default {
    validate({params}) {
        return /^\d+$/.test(params.id)
    },
    async asyncData({$axios, params}) {
        const user = await $axios.$get('http://jsonplaceholder.typicode.com/users/' + params.id)
        return {user}
    },
    layout: 'empty'
}
</script>

<style scoped>

h1{
    color: blue;
    font-size: 54px;
    padding-top: 110px ;
    padding-right: 180px;
}
h3{
    color: rgb(34, 34, 133);
    font-size: 34px;
    padding-top: 51px ;
    padding-left: 44px;
    font-family: 'Times New Roman', Times, serif;
    font-style: italic;
}
h4{
    color: rgb(1, 1, 114);
    font-size: 24px;
    padding-top: 40px ;
    padding-left: 95px;
}

li{
    padding-top: 160px;
    padding-left: 145px;
    list-style: none;
    font-family: helvetica, arial, sans-serif;
    font-size: 17px;
    color: rgb(3, 7, 44);
}

</style>