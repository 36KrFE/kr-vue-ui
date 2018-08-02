<template>
  <div class="hello" @click="show">
    hello
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      name: 'Amy'
    }
  },
  methods: {
    show() {
      const arr = [12,3,2,14,34];
      let newArr = arr.filter(item => {
        return item > 5;
      });
      console.log(newArr);

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
  .hello {
    font-size: 20px;
    color: red;
  }
</style>
