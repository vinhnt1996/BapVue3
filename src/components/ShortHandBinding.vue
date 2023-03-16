<template>
    <div>
        <h3 :id="headingId">{{ name }}</h3>
        <button :disabled="isDisabled">Button</button>
    </div>
</template>
<script>
export default {
    name: 'ShortHandBinding',
    data() {
        return {
            name: 'ShortHandBinding',
            headingId: 'heading',
            classElement :'class_red',
            isDisabled: false,
        }
    }
}
</script>
<style lang="">
    
</style>