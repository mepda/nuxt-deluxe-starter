<template>
  <div class="About__Container">
    <h1 class="title is-1 Title__Text">This is About Page</h1>
    <div class="Card__Container">
      <div class="card" data-aos="fade-right" v-for="d in data" :key="d.id">
        <div>
            <p class="title is-4">{{ d.title }}</p>
        </div>
        <div class="card-content">
          <div class="content">
            {{ d.description }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {

  data(){
    return{
      data : [
        {id:1, title: 'First', description: 'This is first description' },
        {id:2, title: 'Second', description: 'This is second description' },
        {id:3, title: 'Third', description: 'This is third description' },
        {id:4, title: 'Fourth', description: 'This is fourth description' },
        {id:5, title: 'Five', description: 'This is fifth description' },
        {id:6, title: 'Six', description: 'This is sixth description' },
        {id:7, title: 'Seven', description: 'This is seventh description'},
      ]
    }
  }

};
</script>


<style scoped>
.Title__Text {
  text-align: center;
  margin: 15px;
}
.card {
  width: 300px;
  height: 550px;
  margin: 10px;
  background: green;
}
.Card__Container {
  display: flex;
  justify-content: space-evenly;
  flex-flow: wrap row;
  align-items: center;
  padding: 15px;
}
</style>
