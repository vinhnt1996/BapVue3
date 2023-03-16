<template>
    <div>
        BindingStyle
        <p v-bind:style="{
        color:hilightColor,
        backgroundColor: backColor,
        fontSize:headSize + 'px'
    }">Binding Style alone</p>
    <p v-bind:style="headerStyleObject">Binding Style Object</p>
    </div>
</template>
<script>
export default {
    name: 'BindingStyle',
    data() {
        return {
            hilightColor: 'orange',
            backColor: 'red',
            headSize: 50,
            headerStyleObject: {
                fontSize : '50px',
                color: 'green',
                padding: '20px'
            }
        }
    }
}
</script>
<style lang="">
    
</style>