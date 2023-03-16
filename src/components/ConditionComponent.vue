<template>
    <div>
       <h2 v-if="number === 0">The number is zero</h2>
       <h2 v-else-if="number < 0">The number is negative</h2>
       <h2 v-else-if="number > 0"> The number is positive</h2>
       <h2 v-else>The number is not zero</h2>
    </div>
</template>
<script>
export default {
    name: 'ConditionComponent',
    data() {
        return {
            number: 3
        }
    }
}
</script>
<style>
    
</style>