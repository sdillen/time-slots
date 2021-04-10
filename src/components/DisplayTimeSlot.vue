<template>
  <div>
    <b-card>
      <b-row>
        <b-col cols="2">
          {{timeSlot}}
        </b-col>
        <b-col cols="10">
          <ul>
            <li v-for="split in slotSplits" :key="split">
              {{split}}
            </li>
          </ul>
        </b-col>
      </b-row>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'display-time-slot',
  props: {
    timeSlot: {
      type: String,
      require: true
    },
    time: {
      type: Number,
      default: 5
    }
  },
  computed: {
    slotSplits () {
      const split = 60 / this.time
      const splits = []
      for (var i = 0; i <= split; i++) {
        const timeSplit = i * this.time
        splits.push(timeSplit)
      }
      return splits
    }
  }
}
</script>
