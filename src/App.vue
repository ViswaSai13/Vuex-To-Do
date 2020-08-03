<template>
  <div class="container">
    <h1>To-Do List</h1>
    <div id="app">
      <div>
        <TodoNew />
        <TodoList />
      </div>
    </div>
    <h6>Done Using Vuex Store<br>(Please view in Full Screen)</h6>
  </div>
</template>

<script>
import TodoNew from "@/components/TodoNew.vue";
import TodoList from "@/components/TodoList.vue";

export default {
  components: {
    TodoNew,
    TodoList
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Open+Sans");
@import url("https://fonts.googleapis.com/icon?family=Material+Icons");

html {
  font-family: "Open Sans", sans-serif;
  height: 100%;
  color: #333;
}

body {
  background-image: url('./assets/notepad.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: contain;
  background-position: center;  
  display: flex;
  height: 100%;
  margin: 0;
}

.container {
  width: 20rem;
  margin-top: 8rem;
  margin-left: 38.5%;
  padding: 1rem;
}

h1 {
  text-align: center;
  margin-top: 0;
}

h6 {
  text-align: right;
  font-style: italic;
  margin-top: 0;
}

</style>
