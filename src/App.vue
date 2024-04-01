<template>
  <div>
	<h1>Rick and Morty</h1>
  <FilterByStatus/>
  <FilterByName/>
  <ListCharacters/>
  </div>
</template>

<script>
import FilterByStatus from './components/FilterByStatus.vue';
import ListCharacters from './components/ListCharacters.vue';
import FilterByName from './components/FilterByName.vue';

export default {
  name: 'App',
  components: {
    FilterByStatus,
    FilterByName,
    ListCharacters
    
}
}
</script>

<style lang="scss">
:root{
  --background-body: #24282f;
  --background-card: #3c3e44;
  --text-white: white;
  --text-gray: gray;
  --text-orange: orange;
}

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body{
  background-color: var(--background-body);
  color:var (var(--text-white));
  font-family: 'Segoe UI', Tahoma;
}

h1{
  margin-bottom: 3rem;
  text-align: center;
}

.container{
  width: 980px;
  max-width: 90%;
  margin: 5rem auto
}

img{
  width: 100%;
}
</style>
