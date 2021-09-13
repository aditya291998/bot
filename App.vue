/* eslint-disable import/no-unresolved */
/* eslint-disable import/no-unresolved */
<template>
<header>
  <nav>
    <ul>
      <li class="nav-item">
        <router-link class="nav-link" to="/" exact>
        <img class="logo" src="./assets/robot-home.png"/>
        BUILD-A-BOT
         </router-link>
        </li>
        <li class="nav-item">
        <router-link class="nav-link" to="/build" exact>
        BUILD
         </router-link>
        </li>
        <li class="nav-item cart">
        <router-link class="nav-link" to="/cart" exact>
         </router-link>
        </li>
      </ul>
    </nav>
  </header>
  <div class="container">
 <aside class="aside">
   <router-view name="sidebar"/>
    </aside>
  </div>
  <main>
   <router-view/>
    <!-- <Search/> -->
  </main>
</template>

<script>

export default {
  name: 'App',
};
</script>
<style>
body{
  background : linear-gradient(to bottom,#555,#999);
  background-attachment: fixed;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
main {
  padding : 30px;
  background-color: white;
  width: 964px;
  min-height: 300px;
}
header {
  background-color: #999;
  width: 1184px;
  margin: 0 auto;
}
ul {
  padding: 3px;
  display: flex;
}
.nav-item {
  display: inline-block;
  padding: 5px 10px;
  font-size: 22px;
  border-right: 1px solid #bbb;
}.nav-item.cart {
  position: relative;
  margin-left: auto;
  border-right: green;
}
.logo {
  vertical-align: middle;
  height: 30px;
}.router-link-active{
  color: white;
}.nav-link{
  text-decoration: middle;
  color:inherit;
}.container {
  display: flex;
  margin: 10px auto 0 auto;
  justify-content: left;
}.aside {
  padding: 30px;
  background-color: #aaa;
  width:100px;
  min-height: 300px;
}
</style>
