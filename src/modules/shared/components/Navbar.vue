<template>
    <div>
        <router-link :to="{ name: 'home' }">Pokemon List</router-link>
        <router-link :to="{ name: 'pokemon-id', params: { id: '123' }}">Pokemon By Id</router-link>
        <router-link :to="{ name: 'about' }">About Page</router-link>
    </div>
</template>

<style scoped>
div {
    padding: 0 30px;
}
div a {
    font-weight: bold;
    color: #2c3e50;
    margin: 0 10px;
}

a .router-link-exact-active {
    color: #42b983;
}
</style>