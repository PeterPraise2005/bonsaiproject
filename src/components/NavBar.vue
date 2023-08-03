<template>
  <div class="container-fluid">
   <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Bonsai Project</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <route-link to="/" class="nav-link" aria-current="page" href="#">Home</route-link>
        </li>
        <li class="nav-item">
          <router-link to="/about" class="nav-link" href="#">About Us</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/myproduct" class="nav-link" href="#">Product</router-link>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown link
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
            <li><router-link to="/indoor" class="dropdown-item" href="IndoorView.vue">Indoor</router-link></li>
            <li><router-link to="/outdoor" class="dropdown-item" href="#">Outdoor</router-link></li>
            <li><router-link to="/care" class="dropdown-item" href="#">Care</router-link></li>
            <li><router-link to="/account" class="dropdown-item" href="#">Account</router-link></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>
  </div>
</template>