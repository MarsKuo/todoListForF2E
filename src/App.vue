<template>
<div id="app">
    <div class="bg-primary">
      <div class="container justify-content-between d-flex todo-nav">
         <a href="#" class="active" >My Task</a>
        <a href="#">In Progress</a>
        <a href="#">Completed</a>
      </div>
    </div>
    <div class="container my-4">
      <div class="position-relative">
        <i class="fas fa-plus fa-lg text-black-50 position-absolute" style="left: 1rem; top: 1.15rem"></i>
        <input type="text" class="form-control form-control-lg pl-5"
          >
      </div>

      <div class="mt-4">
          <MyEditItem
          ></MyEditItem>

          <div >
            <MyItem
            ></MyItem>
            <MyEditItem ></MyEditItem>
          </div>
      </div>

    </div>

  </div>
</template>

<script>
import MyItem from './components/Item'
import MyEditItem from './components/EditItem'

export default {
  name: 'App',
  components: {
    MyItem,
    MyEditItem
  }
}
</script>

<style>

</style>
