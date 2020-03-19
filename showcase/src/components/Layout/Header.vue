<template>
    <header class="header">
        <h2>RPI Project Showcase</h2>
        <div class="topnav">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">Projects</router-link>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped>
    h2 {
        background: #da1e05 
        linear-gradient(180deg,#e0402b,#da1e05) 
        repeat-x!important;
        color: #ffffff;
        margin: 0px;
    }

    /* .header {
    background: #9ea2a2;
    color: #fff;
    text-align: center;
    padding: 10px;
  }
    .header a {
      color: #fff;
      padding-right: 5px;
      text-decoration: none;
    } */

    /* Add a black background color to the top navigation */
.topnav {
  background-color: #333;
  overflow: hidden;
}

/* Style the links inside the navigation bar */
.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
  background-color: #4CAF50;
  color: white;
}
</style>