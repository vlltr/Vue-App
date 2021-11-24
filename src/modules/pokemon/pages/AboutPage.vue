<template>
    <h1>AboutPage</h1>
    <h2>{{ name }}</h2>
    <button @click="onChangeName">
        Change Name
    </button>
</template>

<script>
export default {

    data() {
        return {
            name: 'Mauro'
        }
    },

    methods: {
        onChangeName() {
            this.name = 'Jose'
        }
    },

    beforeCreate() {
        console.log('beforeCreate')
    },
    created() {
        console.log('created')
    },
    beforeMount() {
        console.log('beforeMount')
    },
    mounted() {
        console.log('mounted')
    },
    beforeUpdate() {
        console.log('beforeUpdate')
    },
    updated() {
        console.log('updated')
    },
    activated() {
        console.log('activated')
    },
    deactivated() {
        console.log('deactivated')
    },
    beforeUnmount() {
        console.log('beforeUnmount')
    },
    unmounted() {
        console.log('unmounted')
    },
    errorCaptured() {
        console.log('errorCaptured')
    },
    renderTracked() {
        console.log('renderTracked')
    },
    renderTriggered() {
        console.log('renderTriggered')
    },
}
</script>
