<template>
  <div class="navigation">
    <ul>
      <li><router-link :to="{name: 'home'}" exact>Home</router-link></li>
      <li><router-link :to="{name: 'products'}" exact>Products</router-link></li>
      <li><router-link :to="{name: 'gallery'}" exact>Gallery</router-link></li>
      <li><router-link :to="{name: 'contact'}" exact>Contact</router-link></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'AppNavigation'
}
</script>

<style>
  .navigation {
    float: right;
  }
  .navigation ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .navigation ul:after {
    content: "";
    display: block;
    clear: box;
  }
  .navigation li {
    float: left;
    width: 100px;
  }
  .navigation a {
    display: block;
    text-align: center;
    text-decoration: none;
    color: white;
    font-size: 22px;
    font-weight: bold;
    font-family: 'Lato';
    line-height: 60px;
  }
  .navigation a:hover {
    background-color: lightskyblue;
    color: darkslateblue;
  }
</style>
