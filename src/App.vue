<template>
  <div id="app">
    <app-navbar/>
    <b-container fluid>
      <b-row>
        <b-col cols="2">
          <app-sidebar/>
        </b-col>
        <b-col cols="10">
          <p>
            These are your tasks for <display-current-day/>
          </p>
          <display-time-table/>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import DisplayCurrentDay from './components/DisplayCurrentDay.vue'
import DisplayTimeTable from './components/DisplayTimeTable.vue'

export default {
  name: 'time-slots',
  components: { DisplayCurrentDay, DisplayTimeTable }
}
</script>
