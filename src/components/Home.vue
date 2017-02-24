<template>
<div class="hello">
   <h3>Home</h3>
   <el-button @click="this.gotoHome">Back</el-button>
</div>
</template>

<script>
import router from '../router';

export default {
   name: 'hello',
   data() {
      return {
         msg: '',
      };
   },
   methods: {
      gotoHome() {
         // eslint-disable-next-line
         // console.console.log('gotoHome');
         router.push('/');
      },
   },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
   font-weight: normal;
}

ul {
   list-style-type: none;
   padding: 0;
}

li {
   display: inline-block;
   margin: 0 10px;
}

a {
   color: #42b983;
}
</style>
