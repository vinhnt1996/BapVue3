<template>
    <div>
        <h2>{{ 2+3+5 }}</h2>
        <h2>{{ 4+8+10+15 }}</h2>
        <h2>Easy function -- {{  add() }}</h2>
        <h2>Multiple function -- {{ mutiples(5) }}</h2>
        <h2>Multiple function -- {{ mutiples(number) }}</h2>
    </div>
</template>
<script>
export default {
    name: 'MethodComponent',
    data() {
        return {
            mutiple: 10,
            number: 15
        }
    },
    methods: {
        add() {
            return 1+2+3;
        },
        mutiples(num) {
            return num * this.mutiple
        }
    }
}
</script>
<style>
    
</style>