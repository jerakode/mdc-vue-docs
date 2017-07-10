<template>
  <header>
    <div class="container">

      <nuxt-link class="logo" to="/" title="Vue MDC Adapter">Vue MDC Adapter</nuxt-link>

      <nav class="menu">
        <ul class="menu-list">
          <li class="menu-item">
            <nuxt-link class="menu-link" to="/components">Components</nuxt-link>
          </li>
          <li class="menu-item">
            <nuxt-link class="menu-link" to="/documentation">Documentation</nuxt-link>
          </li>
          <li class="menu-item">
            <a class="menu-link" href="https://github.com/stasson/vue-mdc-adapter">View at GitHub</a>
          </li>
        </ul>
      </nav>

    </div>
  </header>
</template>

<style lang="scss" scoped>
@import "~assets/styles/_variables.scss";

header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 5em;
  background-color: $main-dark-color;
  color: $main-white-color;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  position: relative;
  margin-left: 4em;
  color: $main-white-color;
  text-decoration: none;
  &:before {
    content: '';
    position: absolute;
    top: -0.5em;
    left: -4em;
    width: 3em;
    height: 3em;
    background-image: url('https://material.io/components/images/mdc-logo.svg');
    // background-color: $main-firm-color;
    background-size: 3em;
    background-position: center;
    background-repeat: no-repeat;
  }
  // width: ;
  // height: 3em;
}

.menu {
  // display: none;
  // width: 100%;
  display: flex;
  // width: auto

}

.menu-list {
  padding: 0;
  margin: 0;
  list-style: none;
  width: 100%;
  display: flex;
  width: auto;
  transition: all 150ms linear;

}

.menu-item {
  line-height: 1;
  flex:1;
  text-align: center;

}

.menu-link {
  margin: 1em 1em;
  display: inline-block;
  font-size: 1em;
  color: $main-white-color;
  text-transform: uppercase;
  text-decoration: none;
  text-align: center;
  white-space: nowrap;
  transition: all 150ms linear;
  &:hover {
    color: $main-firm-color;
    // background: $main-dark-color;

  }
  &:active {
    color: $main-firm-color;
    // background: $main-dark-color;

  }

}

.menu-link.nuxt-link-active, .menu-link.nuxt-link-active:hover {
  color: $main-firm-color;
  transition: all 150ms linear;
  border-bottom: 1px dotted $main-firm-color;

}
</style>
