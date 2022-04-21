<template>
  <div>
    <input type="text" ref="lol">
    <button @click="myfunctions">Посчитать скидку</button>
    <div>{{ check }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      check: 0
    }
  },

  methods: {
    myfunctions(){
      let check = this.$refs.lol.value;
      this.check = check >= 750 ? check - check * 0.05 : check;
    }
  }
};
</script>

<style>

</style>