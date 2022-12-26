<template>
<nav class="navbar fixed-top navbar-light bg-light">
  <div class="container-fluid">
    <router-link to='/'><a class="navbar-brand"><img src="https://mint-sync.netlify.app/logo/logo.png"/><span>Wallet Connect</span></a></router-link>
    <form class="d-flex" role="search">
      <router-link to="/about"><button class="btn btn-primary" type="submit">Connect</button></router-link>
    </form>
  </div>
</nav>
  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Titillium+Web:ital,wght@1,300&display=swap');
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-family: 'Titillium Web', sans-serif !important;
  font-weight:600;
  line-height: 30px;
  word-spacing: 5px;
}
  .navbar-brand img{
    height:40px;
    width:50px;
  }
  .navbar-brand span{
    font-weight:bolder;
    font-size:18px;
    padding:10px;
  }
  nav{
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
  nav .btn{
    width:100%;
    font-size:20px;
    font-size:15px;
    text-transform: uppercase;
  }
  a{
    text-decoration:none !important;
  }
</style>
