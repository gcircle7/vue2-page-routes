<template>
  <v-container>
    <p class="display-1 m-4">서브 페이지1입니다.</p>
    <v-divider></v-divider>
    <p class="display-4 my-4">서브 페이지2입니다.</p>
    <p class="height:100px;">{{ contents_body }} <br/>
      contents_url: {{ contents_url }}</p>
    <div class="text-center">
      <v-btn fab large class="mt-5" color="teal" dark @click="goBack">
        <v-icon>mdi-replay</v-icon>
      </v-btn>
    </div>
  </v-container>
</template>

<script>

export default {
  name: 'sub_page',

  data: () => {
    return {
      contents_body: 'Sub contents',
      contents_url: 'https://vuetifyjs.com'
    }
  },
  methods: {
    goBack: function () {
      this.$router.push('/main')
    }
  }
}
</script>
