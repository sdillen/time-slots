<template>
  <div>
    <b-row v-for="hour in hours" :key="hour">
      <b-col>
        <display-time-slot :timeSlot="hour" :time="5"/>
      </b-col>
    </b-row>
  </div>
</template>

<script>
import DisplayTimeSlot from './DisplayTimeSlot.vue'
export default {
  components: { DisplayTimeSlot },
  name: 'display-time-table',
  data () {
    return {
      hours: [
        '00:00',
        '01:00',
        '02:00',
        '03:00',
        '04:00',
        '05:00',
        '06:00',
        '07:00',
        '08:00',
        '09:00',
        '10:00',
        '11:00',
        '12:00'
      ]
    }
  }
}
</script>
