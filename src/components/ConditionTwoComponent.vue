<template>
    <div>
        <div v-if="display">
            <h2>Vishwas</h2>
            <h2>Codevolution</h2>
            <h2>Vue</h2>
        </div>
        <h2 v-show="true">Using v-show</h2>
        <h2 v-if="showElement">Using v-if</h2>
    </div>
</template>
<script>
export default {
    name: 'ConditionTwoComponent',
    data() {
        return {
            display: true,
            showElement:  false
        }
    }
}
</script>
<style lang="">
    
</style>