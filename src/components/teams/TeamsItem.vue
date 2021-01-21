<template>
  <li>
    <h3>{{ name }}</h3>
    <div class="team-members">{{ memberCount }} Members</div>
    <a href="#">View Members</a>
  </li>
</template>

<script>
export default {
  props: ['name', 'memberCount']
};
</script>

<style scoped>
li {
  margin: 1rem 0;
  /* box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15); */
  padding: 1rem;
  border: 1px solid #ccc;
}

li h3 {
  margin: 0.5rem 0;
  font-size: 1.25rem;
}

li .team-members {
  margin: 0.5rem 0;
}

a {
  text-decoration: none;
  color: white;
  display: inline-block;
  padding: 0.5rem 1.5rem;
  background-color: #d73134;
}

a:hover,
a:active {
  background-color: #df5a5d;
}
</style>
