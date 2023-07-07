<template>
  <div id="app">
    <header>
      <nav>
        <ul>
          <li><router-link to="/">Weather</router-link></li>
          <li><router-link to="/location">Location</router-link></li>
          <li><router-link to="/stopwatch">Stopwatch</router-link></li>
          <li><router-link to="/tictactoe">Tic Tac Toe</router-link></li>
          <li><router-link to="/photo">Photo</router-link></li>
        </ul>
      </nav>
    </header>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
#app {
  text-align: center;
}

header {
  background: linear-gradient(45deg, #2980b9, #6dd5fa);
  padding: 20px;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

nav li {
  display: inline-block;
  margin-right: 10px;
}

nav a {
  color: #fff;
  text-decoration: none;
  padding: 5px 10px;
  font-weight: bold;
  font-size: 18px;
  text-transform: uppercase;
  transition: 0.3s ease;
}

nav a:hover {
  text-decoration: none;
  background: #fff;
  color: #2980b9;
  border-radius: 5px;
}
</style>
