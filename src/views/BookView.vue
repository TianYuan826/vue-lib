<template>
  <div class="book-view">
    <h1>This is an about page</h1>
    <table class="book-table">
      <tr>
        <td>No.</td>
        <td>Title</td>
        <td>Author</td>
      </tr>
      <tr v-for="item in books">
        <td></td>
      </tr>
    </table>
  </div>
</template>
<script>
import header from '@/components/header.vue'

export default {
  name: 'BookView',
  components: {
    header
  },
  data(){
    return{
      books:[]
    }
  }
}
</script>
<style scoped>
.book-table{
  border: 1px solid black;
}
</style>