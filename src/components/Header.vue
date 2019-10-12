<template>
  <div class="header container">
    
    <h1 class="my-5">
      <router-link to="/" class="title">Gucci Code</router-link>
    </h1>
    <div class="clearfix mb-4">
    <font-awesome-icon :icon="['fab', 'github-square']" class="icon mr-3" />
    <font-awesome-icon :icon="['fab', 'facebook-square']" class="icon" />

    </div>
    <ul class="nav justify-content-end mb-5 lp-menu">
      <li v-for="(item, index) in items" :key="index" class="nav-item">
        <router-link v-bind:to="item.path" class="nav-link none">{{ item.title }}</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      isActive: true,
      items: [
        { title: "About", path: "/about" },
        { title: "Works", path: "/works" },
        { title: "Skills", path: "/skills" },
        { title: "Contact", path: "/contact" }
      ]
    };
  },
  methods: {
    toggle_class: function() {
      this.isActive = !this.isActive;
    }
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Mansalva&display=swap");

@media (max-width: 767.98px) {
  .lp-menu {
   width: 100%;
  }
  .nav-item {
    min-width: 108px;
    width: 50%;
    padding: 9px;
    border: 1px solid rgba(170, 158, 158, 0.199);
    text-align: center;
  }
}

@media (min-width: 768px) {
}

.title {
  font-family: "Mansalva", cursive;
  color: rgb(32, 29, 29);
  text-decoration: none;
}

.router-link-exact-active.none {
  color: #000;
  opacity: 0.3;
}

.none {
  color: #000;
}

.icon {
  font-size: 3rem;
  padding: 2px;
  float: right;
}
</style>