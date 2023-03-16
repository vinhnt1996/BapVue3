<template>
    <div>
        <h2>{{ channel }}</h2>
        <h2 v-html="channel"></h2>
        <h3 v-html="hack"></h3>
    </div>
</template>
<script>
export default {
    name: 'BindingHtml',
    data() {
        return {
            channel: '<b>Binding HTML</b>',
            hack: `<a href="#" onclick="alert('You have been hacked!')">Win a prize!</a>`
        }
    }
}
</script>
<style lang="">
    
</style>