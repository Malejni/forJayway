<template>
  <div class="hello">
    <div class="header">
      <img src="../assets/logo.png">
      <h1>Welcome to my Quiz</h1>
    </div>
    <div class="content">
      <p>This quiz is made with Vue.js and contains 10 questions that you
        will have 15 seconds to choose 1 of 4 alternatives to answer. We
        offer you 2 lifelines, 50/50 and +10sec, so hopefully you'll be
        able to solve all the questions. 
      </p>
      <h3>Good luck!</h3>
    </div>
    <div class="content-button">
      <button v-on:click="counter++">Start quizzing {{counter}} times!</button>
    </div>
    <div class="footer">
      <p>by Malena Brinkheden 2018</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      counter: 0
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  display: grid;
  grid-template-areas: "header" "header"
  "content" "content"
  "content2" "content2"
  "footer" "footer";
  grid-template-columns: auto;
  grid-template-rows: auto;
}

.header {
  grid-area: header;
  margin-top: 60px;
  text-align: center;
  color: #2c3e50;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}

h1, h3 {
  font-weight: normal;
}

.content {
  grid-area: content;
  text-align: center;
  color: #2c3e50;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
} 

.content-button {
  grid-area: content2;
  text-align: center;
}

.footer {
  grid-area: footer;
  color: grey;
  font-size: 12px;
  text-align: center;
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
}
</style>
