<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title class="headline">
          TyBscIT MCQ Mock Test
        </v-card-title>
        <v-card-text>
          <v-text-field v-model="roll_no" outlined label="Roll No" dense />
          <v-combobox
            outlined
            label="Subject"
            v-model="subject"
            dense
            :items="items"
          />
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn color="primary" nuxt @click="navigate">
            Start
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    Logo,
    VuetifyLogo
  },
  data() {
    return {
      items: ["BI", "ITSM", "SQA", "EN", "SIC"],
      roll_no: "",
      subject: "BI"
    };
  },
  methods: {
    navigate() {
      this.$router.push("/mcq");
    }
  }
};
</script>
