<template>
  <div>
    {{ str }}
    <app-header v-bind:propsdata="str"
                v-on:renew="renewStr"
    ></app-header>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "App.vue",
  components: {
    "app-header": AppHeader
  },
  data: function() {
    return {
      str: "Header"
    };
  },
  methods: {
    renewStr: function() {
      this.str = "hi";
    }
  }
};
</script>

<style scoped>

</style>