<template>
  <div id="app">
    <ul>
      <li>
        <router-link to="/hello">hello</router-link>
        <router-link to="/pageone">pageone</router-link>
      </li>
    </ul>
    <div>
      <transition enter-active-class="animated zooInLeft" leave-active-class="animated zoomOutRight">
         <router-view></router-view>
      </transition>
    </div>
  </div>
</template>

<script>


export default {
  name: 'app'

}
</script>

<style>
body,html{
  overflow: hidden;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
