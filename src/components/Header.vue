<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <router-link to="/" class="navbar-brand"><a>Stock App</a></router-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <router-link to="/portfolio" class="nav-link" active-class="active"><a>Portfolio</a></router-link>
        <router-link to="/stocks" class="nav-link" active-class="active"><a>Stocks</a></router-link>
      </ul>
      <ul class="navbar-nav ml-auto">
        <li class="nav-item"><a class="nav-link" href="#">End Day</a></li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Save &amp; Load
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">Save Data</a>
            <a class="dropdown-item" href="#">Load Data</a>
          </div>
        </li>
      </ul>
    </div>
  </nav>
</template>
<style>
  .navbar{
    margin: 40px 0;
  }
  .navbar-dark{
    background: #3FC1C9!important;
  }
</style>

