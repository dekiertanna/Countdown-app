<template>
  <md-card md-with-hover>
    <md-card-header>
      <md-field>
        <label>Title of your countdown</label>
        <md-input v-model="title"></md-input>
      </md-field>
     
    </md-card-header>

    <md-card-content>
      <md-datepicker v-model="selectedDate">
        <label>Select date</label>
      </md-datepicker>
       <md-field>
      <label>Time left:</label>
      <md-input v-model="timeLeft" readonly disabled></md-input>
    </md-field>
    </md-card-content>

    <md-card-actions>
      <md-button class="md-primary" :md-ripple="false"
        >Start</md-button>
        <md-button class="md-accent" :md-ripple="false"> Delete</md-button>
    </md-card-actions>
  </md-card>
</template>

<style lang="scss" scoped>
.md-card {
  width: 320px;
  margin: 20px;
  vertical-align: top;
}

.md-field:last-child {
  margin-bottom: 40px;
}
</style>

<script>
export default {
  name: "CounterCard",
  data: () => ({
    title: null,
    selectedDate: null,
    timeLeft: null
  }),
};
</script>
