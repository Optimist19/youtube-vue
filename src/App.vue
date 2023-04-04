<template>
  <div>
    <HeadYt />
    <SideBar />
    <MainYt />
  </div>
</template>

<script>
import HeadYt from './components/Head.vue'
import SideBar from './components/SideBar.vue'
import MainYt from './components/Main.vue'

export default {
  name: 'App',
  components: {
    HeadYt,
    SideBar,
    MainYt
  }
}
</script>

<style>
#app {
  margin: 0;
	padding: 0;
	padding-top: 110px;
	padding-bottom: 200px;
	padding-left: 100px;
	padding-right: 20px;
	background-color:rgb(247, 255, 255);
	animation: fade;
	animation-duration: 3s;
}

@keyframes fade{
	from{opacity: 0;};
	to{opacity: 1;};
}
</style>
