<template>
  <div class="hello">

    <!--<img src="../assets/sunset.jpg" height="854" width="1280" class="bg"/>-->
    <div class="bg">
      <div class="wel">{{ msg }}</div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to bihu'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
  text-align: center;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 ;
}
a {
  color: #42b983;
}
.bg {
  background: url(./../assets/sunset.jpg) no-repeat ;
  display: block;
  width: 100%;
  height: 40rem;
  background-size:100%150%;
  transform: perspective(62.5rem) translateZ(0);
  transition:  8s;
  border-style: none;

}
.bg:hover {
  transform: perspective(62.5rem) translateZ(12.25rem);
  transition:  8s;
}
  .wel{
    color: white;
    text-align: center;
    font-size:4.125rem;
    height: 3.125rem;
    transform: translate(500px,300px);
    margin-top: -0.625rem;
    font-family: Georgia,Microsoft YaHei,\\5FAE\8F6F\96C5\9ED1,STXihei,\\534E\6587\7EC6\9ED1,serif;
    position: absolute;
  }
@media screen and (max-width: 980px) {
  .wel{
    transform: translate(200px,300px);
  }
  }
@media screen and (max-width: 550px) {
  .wel {
    transform: translate(100px, 300px);
    font-size: 2.125rem;
  }
}
@media screen and (max-width: 300px) {
  .wel{
    transform: translate(100px,200px);
    font-size: 1.325rem;
  }
}

</style>
