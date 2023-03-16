<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Learning basic Vuejs3"/>
    <binding-text></binding-text>
    <BindingHtml />
    <BindingAttribute />
    <BindingClass />
    <BindingStyle />
    <ShortHandBinding />
    <condition-component></condition-component>
    <ConditionTwoComponent /> -->
    <!-- <list-rendering></list-rendering> -->
    <!-- <ListAndKey></ListAndKey> -->
    <!-- <MethodComponent /> -->
    <!-- <event-handling></event-handling> -->
    <new-component></new-component>  
  </div>
</template>

<script>
import NewComponent from './components/NewComponent.vue'
// import EventHandling from './components/EventHandling.vue'
// import ListRendering from './components/ListRendering.vue'
// import BindingText from './components/BindingText.vue';
// import HelloWorld from './components/HelloWorld.vue';
// import BindingHtml from './components/BindingHtml.vue';
// import BindingAttribute from './components/BindingAttribute.vue';
// import BindingClass from './components/BindingClass.vue';
// import BindingStyle from './components/BindingStyle.vue';
// import ShortHandBinding from './components/ShortHandBinding.vue';
// import ConditionComponent from './components/ConditionComponent.vue';
// import ConditionTwoComponent from './components/ConditionTwoComponent.vue';

// import ListAndKey from './components/ListAndKey.vue';
// import MethodComponent from './components/MethodComponent.vue';

export default {
  name: 'App',
  components: {
    NewComponent
    // EventHandling
    // MethodComponent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
