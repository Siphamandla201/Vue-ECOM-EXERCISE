<template lang="">
    <div>
        <nav>
            <div>
                <img src="https://i.pinimg.com/236x/44/c9/9c/44c99c63636fff398dda0885ff170d36.jpg" alt="logo">
            </div>
            <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/product">Product</router-link></li>
            <li><router-link to="/about">About</router-link></li>
            <li><router-link to="/admin">Admin</router-link></li>
            <li><router-link to="/contact">Contact</router-link></li>
        </ul>
        </nav>
        <router-view/>
    </div>
</template>
<script>
export default {
    name: 'Navbar'
}
</script>
<style>

nav {
  padding: 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #2c3e50;
}

nav > ul {
  display: flex;
  align-items: center;
  list-style: none;
}

nav > ul > li {
    margin-right: 15px;
    color: red;
}

nav > ul > li > a {
    font-weight: bold;
    color: #42b983;
text-decoration: none;
}

nav > ul > li  > a.router-link-exact-active {
  color: #49715f;
  border-bottom: 3px solid #49715f ;
}
    
</style>