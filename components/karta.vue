
<template>
  <div class="bot">
    <div class="name">
      {{kartochka.author.name }}
    </div>
    <div class="photo">
      <img :src="kartochka.author.photo" />
    </div>
    <div class="title">
      {{kartochka.title}}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    kartochka: {
      type: Object,
      default: () => {}
    },
}

}
</script>

<style scoped>

.bot {
  padding: 20px;
}



.photo {
  display: flex;
  flex-direction: row;
  width: 100%;
}

img {
  width: 100%;
}

.name{

font-weight: 400;
font-size: 24px;
line-height: 36px;
color: #000000;

}
</style>