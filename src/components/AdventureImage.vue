<template>
  <div><img class="img-fluid" src="@/assets/hobbit-home.jpg" /></div>
  <div>
    <img class="img-fluid" :src="require(`@/assets/${images[index]}.jpg`)" />
  </div>
  <button @click="changeIndex()">Click Me!</button>
</template>

<script>
export default {
  name: "Image",
  data() {
    return {
      images: ["alps", "bendemeer-estates", "dirt-road", "fireplace", "forest-path", "forest1", "forest2", "grass-plains", "lonely-mountain", "mountains1", "mountains2", "path1", "path2", "waterfall"],
      index: 0
    };
  },
  methods: {
    changeIndex() {
      this.index = Math.floor(Math.random() * (this.images.length));
  console.log(this.index);   }
  }
};
</script>
