<template>
  <div class="container">
    <div class="form">
      <div class="siimple-h3">Add a New Link </div>
      <div>
        <label class="siimple-label">Title </label>
        <input  v-model="form.title" type="text" class="siimple-input" placeholder="Github">
      </div>
      <div>
        <label class="siimple-label">URL</label>
        <input v-model="form.url" type="text" class="siimple-input" placeholder="https://github.com/">
      </div>
      <div class="save-button-container">
        <div @click="addLink" class="siimple-btn siimple-btn--blue">Add</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'NewLink',
    data () {
      return {
        form : {
          title: '',
          url: ''
        }
      }
    },
    methods: {
      addLink: function () {
        let link = {
          title: this.form.title,
          url: this.form.url
        }
        // we gonna replace this console log with  a socket client call
        console.log(link)
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .form {
    width: 300px;
    height: auto;
    background: white;
    border-radius: 5px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    padding: 50px;
    text-align: center;
    box-shadow: 1px 2px 5px #dbdbdb;
    position: sticky;
    top: 0;
  }

  .siimple-input {
    height: 35px;
    margin: 15px;
  }

  .siimple-btn--blue {
    background-color: #4894f0;
    color: #fff;
    width: 216px;
    height: 45px;
    margin: 15px;
    display: flex;
    justify-content: center;
    align-self: center;
    align-items: center;
    justify-content: space-around;
  }
  .save-button-container {
    display: flex;
    justify-content: center;
  }

</style>
