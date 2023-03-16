<template>
    <div>
        <h3 v-bind:id="headingId">{{ name }}</h3>
        <h3 v-bind:class="classElement" v-text="name"></h3>
        <button v-bind:disabled="isDisabled">Button</button>
    </div>
</template>
<script>
export default {
    name: 'BindingAttribute',
    data() {
        return {
            name: 'Binding Attribute',
            headingId: 'heading',
            classElement :'class_red',
            isDisabled: false,
        }
    }
}
</script>
<style lang="">
    
</style>