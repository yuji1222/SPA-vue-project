<template>
  <div id="overlay" v-on:click="clickEvent">
    <div id="content" v-on:click="stopEvent">
      <p><slot></slot></p>
      <button v-on:click="clickEvent">close</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "openmodal",
  methods: {
    clickEvent: function(){
      this.$emit('form-child')
    },
    stopEvent: function(){
      event.stopPropagation()
    }
  }
};
</script>

<style scoped>
#overlay {
  z-index: 1;

  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);

  display: flex;
  align-items: center;
  justify-content: center;
}

#content {
  z-index: 2;
  width: 50%;
  padding: 1em;
  background: #fff;
}
</style>
