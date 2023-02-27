<template>
  <div class="nav">
    <h1>Whilmar</h1>
    <ul>
      <li v-for="link in links" :key="link.id">
        <a :href="link.url">{{ link.name }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      links: [
        {
          id: 1,
          name: 'Home',
          url: '/'
        },
        {
          id: 2,
          name: 'About',
          url: '/about'
        },
        {
          id: 3,
          name: 'Contact',
          url: '/contact'
        }
      ]
    }
  }
}
</script>

<style scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  /*background-color: #fff;*/
  padding: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

ul {
  display: flex;
  list-style-type: none;
}

li {
  margin-right: 10px;
}

a {
  text-decoration: none;
  color: #333;
}

a:hover {
  color: #007aff;
}
</style>
