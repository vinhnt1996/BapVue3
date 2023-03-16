<template>
    <div>
        <h3 v-text="text" v-bind:class="classElement"></h3>
        <h2 v-bind:class="status">Status</h2>
        <h3 v-bind:class="isPromoted && 'promoted'">Promoted Movie</h3>
        <h3 v-bind:class="isSoldout ? 'sout-old' : 'new'">Soldout? movie</h3>
        <h2 v-bind:class="['new', 'sout-old']"> Newly promoted movie</h2>
    </div>
</template>
<script>
export default {
    name: 'BindingClass',
    data() {
        return {
            text: 'Underline text',
            classElement: 'underline',
            status: 'danger',
            isPromoted: false,
            isSoldout: true
        }
    }
}
</script>
<style scoped>
    .underline {
        color:red;
        font-size: 18px;
    }
    .status {
        color: red;
        font-size: 35px;
    }
    .promoted {
        color: gray;
    }
    .new {
        font-style: bold;
    }
    .sout-old {
        font-style: italic;
    }
</style>