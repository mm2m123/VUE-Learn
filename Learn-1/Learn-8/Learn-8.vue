<body>
    <div id="hello-vue" class="m-3 p-3 border border-success">
        {{ x + y }}
    </div>
    <script>
Vue.createApp({
  /* options */
  data() {
    return {
      x: 10,
      y: 20,
    };
  },
  created() {
    // 组件生成时
    console.log("x + y is: " + (this.x + this.y));
  },
}).mount("#hello-vue");
</script>
</body>