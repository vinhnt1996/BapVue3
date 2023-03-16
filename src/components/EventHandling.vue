<template>
    <div>
        <h2>Event Handling</h2>
        <h2>{{ name }}</h2>
        <button v-on:click="name ='BatMan'">Change name</button>
        <h2>{{ count }}</h2>
        <button v-on:click="count++">Increment</button>
        <button v-on:click="count--">Decrement</button>
        <button v-on:click="increments(amount)">Increment</button>
        <button v-on:click="decrements(amount)">Decrement</button>
    </div>
</template>
<script>
export default {
    name: 'EventHandling',
    data() {
        return {
            name: 'Bruce',
            count: 0,
            amount: 3
        }
    },
    methods: {
        changeName() {
            return this.name = 'Vinh'
        },
        increments(num) {
            return this.count+=num
        },
        decrements(num) {
           return this.count = this.count-num
        }
    }
}
</script>
<style>
    
</style>