<template>
  <div class="container">
    <div class="feed-container">
      <div class="siimple-h3">Feed</div>
      <div class="siimple-alert siimple-alert--info">
        Github: <span class="siimple-link"> https://github.com/ </span>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Feed'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 80%;
  }

  .feed-container {
    width: 50%;
    height: auto;
    background: white;
    border-radius: 5px;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    padding: 50px;
    text-align: center;
    box-shadow: 1px 2px 5px #dbdbdb;

  }

  .simple-alert {
    letter-spacing: 1.5px;
     width: 50%;
  }
  .siimple-a, .siimple-link {
    color: #fff;
  }
</style>
