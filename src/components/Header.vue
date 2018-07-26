<template>
  <div>
    <nav class="navbar navbar-light">
      <div class="container">
        <router-link class="navbar-brand"
          to="/home">
            Go to Home
        </router-link>
         <ul v-if="!isAuthenticated" class="nav navbar-nav pull-xs-right">
        <li class="nav-item">
          <router-link class="nav-link"
            active-class="active"
            to="/home">
            Home
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link"
            active-class="active"
            to="/login">
            <i class="ion-compose"></i>Sign in
          </router-link>
        </li>
        <li class="nav-item">
          <router-link
            class="nav-link"
            active-class="active"
            to="/register">
            <i class="ion-compose"></i>Sign up
          </router-link>
        </li>
      </ul>
      </div>
    </nav>
  </div>
</template>
