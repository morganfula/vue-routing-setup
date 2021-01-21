<template>
  <header>
    <nav>
      <ul>
        <li>
          <button @click="setActivePage('teams-list')">Teams</button>
        </li>
        <li>
          <button @click="setActivePage('users-list')">Users</button>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  emits: ['set-page'],
  methods: {
    setActivePage(page) {
      this.$emit('set-page', page);
    }
  }
};
</script>

<style scoped>
header {
  width: 100%;
  height: 5rem;
  background-color: #ffe69a;
}

nav {
  height: 100%;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

li {
  margin: 0 2rem;
}

button {
  font: inherit;
  background: transparent;
  border: 1px solid transparent;
  cursor: pointer;
  color: #000;
  padding: 0.5rem 1.5rem;
  display: inline-block;
  outline: none;
}

button:hover,
button:active {
  color: #d73134;
  border-color: #d73134;
  /* background-color: #1a037e; */
}
</style>
