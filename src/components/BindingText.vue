<template>
    <div>
        <h2>{{ greet }} {{  bindingText}}</h2>
        <h2>{{ greet }} {{ name }}</h2>
        <p v-text="channel"></p>
    </div>
</template>
<script>
export default {
    name: 'BindingText',
    data(){
        return {
            bindingText: 'Vinh',
            name: "Batman",
            greet: 'Hello',
            channel: 'Evolution'
        }
    }
}
</script>
<style lang="">
    
</style>