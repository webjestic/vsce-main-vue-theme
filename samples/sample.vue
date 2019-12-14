<template>
    <!-- calendar snippit from https://vuetifyjs.com/en/components/calendars --> 
  <v-sheet height="500">
    <v-calendar
      type="month"
      now="2019-01-08"
      value="2019-01-08"
      :events="events"
    ></v-calendar>
  </v-sheet>
</template>

<script>
  export default {
    data: () => ({
      events: [
        {
          name: 'Vacation', // comments
          start: '2018-12-30',
          end: '2019-01-02',
        },
        {
          name: 'Meeting',
          start: '2019-01-07',
        },
        {
          name: '30th Birthday',
          start: '2019-01-03',
        },
        {
          name: 'New Year',
          start: '2019-01-01',
        },
        {
          name: 'Conference',
          start: '2019-01-21',
        },
        {
          name: 'Hackathon',
          start: '2019-01-30',
          end: '2019-02-01',
        },
      ],
    }),
  }
</script>

<style lang="scss">
nav {
    ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }
  
    li { display: inline-block; }
  
    a {
      display: block;
      padding: 6px 12px;
      text-decoration: none;
    }
  }
</style>