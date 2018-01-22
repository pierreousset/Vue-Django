<template>
    <div id="app">
        <div>
            <h1>{{ msg }}</h1>
            </br>
            <input v-model="newItem">
            <button @click="addItemToList">Add</button>
            <!-- displays list -->
            <ul>
                <li v-for="item in listItems">{{ item }}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'app',
    data () {
        return {
            msg: 'My To Do List',
            listItems: ['buy food', 'play games', 'sleep'],
            newItem: ''
        }
    },
     methods: {
      addItemToList() {
          this.listItems.push(this.newItem);
          this.newItem = '';
      }
  }
}
</script>
