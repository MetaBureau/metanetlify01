<template>
  <div>
    <p class="menu-label is-hidden-touch">General</p>
    <ul class="menu-list">
      <li v-for="(item, key) of items" :key="key">
        <nuxt-link :to="item.to" exact-active-class="is-active">
          <b-icon :icon="item.icon" /> {{ item.title }}
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' },
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' },
        },
        {
          title: 'Gold',
          icon: 'lightbulb',
          to: { name: 'gold' },
        },
        {
          title: 'Rush',
          icon: 'lightbulb',
          to: { name: 'rush' },
        },
        {
          title: 'Hot-Cheese',
          icon: 'lightbulb',
          to: { name: 'hot' },
        },
      ],
    }
  },
}
</script>
