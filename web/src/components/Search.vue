<template>
  <div class="search">
    <h2> I'm looking for a <u>{{lang}}</u> developer in <u>{{location}}</u></h2>
    <div>
      <form>
        <div class="form-group">
          <label for="language">Language</label>
          <input v-model="lang" class="form-control" id="language">
        </div>
        <div class="form-group">
          <label for="location">Location</label>
          <input v-model="location" class="form-control" id="location">
        </div>
        <button type="submit" class="btn btn-primary">Search</button>
    </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Search',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      lang: 'Ruby',
      location: 'Toronto',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
