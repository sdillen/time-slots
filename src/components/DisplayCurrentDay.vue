<template>
  <span>{{currentDay}}</span>
</template>

<script>
export default {
  name: 'display-current-day',
  computed: {
    currentDay () {
      // fetch current date
      const date = new Date()

      // switch through days and respond with day string
      switch (date.getDay()) {
        case 1:
          return 'Monday'
        case 2:
          return 'Tuesday'
        case 3:
          return 'Wednesday'
        case 4:
          return 'Thursday'
        case 5:
          return 'Friday'
        case 6:
          return 'Saturday'
        case 7:
          return 'Sunday'
        default:
          return null
      }
    }
  }
}
</script>
