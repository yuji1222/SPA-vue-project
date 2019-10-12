<template>
  <div class="footer container">
    <ul class="nav justify-content-start mb-5">
      <li v-for="(item, index) in items" :key="index" class="nav-item">
        <router-link v-bind:to="item.path" class="nav-link none">{{ item.title }}</router-link>
      </li>
    </ul>
    <p class="name float-right">© YUJI YANAGISAWA All rights reserved.</p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      items: [
        { title: "About", path: "/about" },
        { title: "Works", path: "/works" },
        { title: "Skills", path: "/skills" },
        { title: "Contact", path: "/contact" }
      ]
    };
  }
};
</script>

<style scoped>
.router-link-exact-active.none {
  color: #000;
  opacity: 0.3;
}

.none {
  color: #000;
}

.name {
  font-size: 0.8rem;
  color: rgba(150, 150, 150, 0.877);
}
</style>