<template>
  <div>
    <b-nav vertical pills>
      <b-nav-item v-for="weekday in week" :key="weekday">
        {{weekday}}
      </b-nav-item>
    </b-nav>
  </div>
</template>

<script>
export default {
  name: 'app-sidebar',
  data () {
    return {
      week: [
        'MO',
        'TU',
        'WE',
        'TH',
        'FR',
        'SA',
        'SU'
      ]
    }
  }
}
</script>
