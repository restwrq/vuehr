<template lang="html">
  <div class="test">
  <article>
    <h1>合同</h1>
    <section class="myarticle">
    <p>
      啊实打实大苏打实打实大苏打实打实大苏打按时大
      苏打实打实大大实打实大苏打实大苏打实打实
      打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
          苏打实打实大大实打实大苏打实大苏打实打实
        打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
            苏打实打实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实啊实打实打算
          大大实打实大苏打实大苏打实打实 打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
          苏打实打实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实
    </p>
  </section>
  <section  class="myarticle">
    <p>
      啊实打实大苏打实打实大苏打实打实大苏打按时大
        苏打实打实大大实打实大苏打实大苏打实打实
        打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
            苏打实打实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
              苏打实打实大大实打实大苏打实大苏打实打实
            打实啊实打实十大大苏打大大实
            大大实打实大苏打实大苏打实打实
            打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
            苏打实打实大大实打实大苏打实大苏打实打实
            打实啊实打实十大大苏打大大实
    </p>
  </section>
  <section class="myarticle">
    <p>啊实打实大苏打实打实大苏打实打实大苏打按时大
        苏打实打实大大实打实大苏打实大苏打实打实
      打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
          苏打实打实大大实打实大苏打实大苏打实打实
        打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
            苏打实打实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实啊实打实大苏打实打实大苏打实打实大苏打按时大
          苏打实打实大大实打实大苏打实大苏打实打实
          打实啊实打实十大大苏打大大实
    </p>
  </section>
  <section class="footer">
    <span class="left">甲方：</span>
    <span class="right">乙方：</span>
  </section>
  </article>
</div>
</template>

<script>
export default {
  data() {
      return {
        workId:'asdas',
        form: {
          name: '',
          region: '',
          date1: '1999-9-9',
          date2: '',
          delivery: false,
          type: [],
          resource: '',
          desc: '',

        }
      }
},
mounted(){
  this.initWorkId()
  console.log("初始化执行了")
},
methods: {
    initWorkId(){
        this.workId= this.$route.query.workId
    },
    onSubmit() {
    alter('submit!');
    }
  }
}
</script>

<style lang="css">
.test{
   text-align: center;
   text-indent: 2em;

}
article{
  position:absolute;
  width: 45%;
  left:30%;
}
.footer{
  position:left;
}
.left{
  position:absolute;
  right: 120px;

}
.right{
  position:absolute;
  left:80px;
}
.myarticle{
  text-align: left;
}

</style>
