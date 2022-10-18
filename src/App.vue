<template>
<div id="app">
      <vs-button
        @click="openNotification">
        Open Notification
      </vs-button>
</div>
</template>

 <script>
    export default {
      methods: {
        openNotification() {
          this.$vs.notification({
            title: 'Q bot',
            text: `These documents refer to the latest version of vuesax (4.0+),
            to see the documents of the previous versions you can do it here 👉 Vuesax3.x`
          })
        }
      }
    }
  </script>


<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
}
html {
  background-color: black;
}

.vs-notification {
  background-color: rgb(53, 53, 53);
  color: white;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  
}

</style>
