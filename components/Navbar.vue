<template>
  <header class="header">
    <img class="header__logo" src="~assets/img/logoo.png"/>
    <nav>
      <ul class="menu">
        <li class="menu__nav-item">
        <nuxt-link class="menu__nav-link menu__nav-link--active" to="/">
          home
        </nuxt-link>
        </li>
        <li>
        <nuxt-link class="menu__nav-link" to="/about">
          about
        </nuxt-link>
        </li>
        <li>
        <nuxt-link class="menu__nav-link" to="/blog">
          blog
        </nuxt-link>
        </li>
        <li>
        <nuxt-link class="menu__nav-link menu__nav-link--last-child" to="/contact">
          contact
        </nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>