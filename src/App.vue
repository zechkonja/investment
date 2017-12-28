<template>
  <div id="app">
    <Container />
  </div>
</template>

<script>
import Container from './components/Container'

export default {
  name: 'app',
  components: {
    Container
  }
}
</script>

<style>

body{
  font-family:'Open-sans', sans-serif;
  font-size:17px;
  line-height:1.5em;
  margin:0;
  padding:0;
}

img{
  width:100%;
}

/* COMMON CLASSES */
.primary-text{
  color:#56a79a;
}

.primary-background{
  background:#56a79a;
}

</style>
