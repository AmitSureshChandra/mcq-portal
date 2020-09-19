<template>
  <v-card elevation="0" class="pa-3 ma-2">
    <v-card-title>
      <v-row> {{ qno }} . {{ question }} </v-row>
    </v-card-title>
    <v-row>
      <v-col
        cols="12"
        class="col-sm-6 col-lg-3"
        v-for="option in options"
        :key="option"
      >
        <!--
        <VRadio
          v-model="answered"
          :label="option"
          :value="true"
          @change="$emit('answer', answered)"
        ></VRadio>

        -->

        <input type="radio" :name="option" />
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
export default {
  name: "Question",
  props: {
    question: String,
    options: Array,
    answer: String,
    qno: String
  },
  data() {
    return {
      answered: ""
    };
  }
};
</script>
