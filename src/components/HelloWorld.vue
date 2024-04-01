<template>
  <div class="big">
    <div class="item" v-for="(map, index) in maps" :key="index">
      <iframe :src="`maps/${map}/index.html`" width="100%" height="500px"></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      maps: ['DistrictMap', 'Map', 'TrashDistrictMap', 'TrashMap']
    }
  },
  mounted() {

  }
}
</script>

<style scoped>
.big {
  display: flex;
  flex-wrap: wrap;
}
.item {
  flex-grow: 1;
}
/* Your styles here */
</style>
