<template>
  <v-container fluid>
    <v-row align="center">
      <v-col md="12" sm="12" cols="12">
        <p class="google-font mb-0" style="font-weight: 350;font-size:200%">
          <b>
            Our
            <span style="color: #1a73e8;">Events</span>
          </b>
        </p>
        <p class="google-font mt-0" style="font-size:120%">
          Questions? Please contact
          <a
            style="color:#1565C0;text-decoration: none;"
            :href="`mailto:${communityData.communityEmail}`"
          >{{communityData.communityEmail}}</a>
        </p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import communityData from "@/assets/data/communityData.json";
export default {
  data() {
    return {
      communityData: communityData
    };
  }
};
</script>