<!--  <template>
   <Card>
    <div class="card">
      <p>Hello There</p>
    </div>
  </Card>
  <Card>
    <template v-slot="cardHeader">
 #cardHeader 
      <p class="lead">Title 1</p>
    </template>
    <template v-slot="cardBody">
      <div class="d flex justify-content-center flex-wrap">
        <img src="" alt="image" loading="lazy">
        <p class="lead"></p>
      </div>
    </template>
    <template>
      <div class="d-flex ">
        <button class="btn btn-primary">View Detail</button>
        <button class="btn btn-primary">Cart</button>

      </div>
    </template>
  </Card>
</template>

<script>
import Card from './components/Card.vue';

export default {
  name: 'App',
  components: {
    Card

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>  -->


<template>
  <div class="card">
   <div class="card-header">
       <slot name="cardHeader"></slot>
   </div>
   <div class="card-body">
       <slot name="cardBody"></slot>
   </div>
   <div class="card-footer">
       <slot></slot>
   </div>
  </div>
</template>

<script>
   export default {
       name: 'CardComp'
   }
</script>

<style scoped>
.card {
   width: 18rem;
   margin: .5rem;
}
</style>