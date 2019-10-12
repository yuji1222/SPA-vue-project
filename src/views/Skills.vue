<template>
  <div class="skills container">
    <button v-on:click="openModal">Click</button>
    <Open-modal v-show="showContent" v-on:form-child="closeModal">slotからモーダルウィンドウへ</Open-modal>
  </div>
</template>

<script>
import OpenModal from "@/components/OpenModal.vue";

export default {
  components: {
    OpenModal
  },
  data() {
    return {
      showContent: false
    };
  },
  methods: {
    openModal: function() {
      this.showContent = true;
    },
    closeModal: function() {
      this.showContent = false;
    }
  }
};
</script>

