<template>
    <div>
        <template v-for="name in names">
            <h2 v-if="name==='Bruce'" :key="name">{{ name }}</h2>
        </template>
    </div>
</template>
<script>
export default {
    name: 'ListAndKey',
    data() {
        return {
            names: ['Bruce', 'Clark', 'Diana']
        }
    }
}
</script>
<style>
    
</style>