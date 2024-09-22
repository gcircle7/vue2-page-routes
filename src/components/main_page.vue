<template>
  <v-container>
    <p class="display-1 m-4">메인 페이지1입니다.</p>
    <v-divider></v-divider>
    <p class="display-4 my-4">메인 페이지2입니다.</p>
    <p> {{ contents_title }}<br/> {{ contents_url }}</p>
    <div class="text-center">
      <v-btn fab large class="mt-5" color="purple" dark to="/sub">
        <v-icon>mdi-arrow-right</v-icon>
      </v-btn>
    </div>
  </v-container>
</template>

<script>

export default {
  name: 'main_page',

  data: () => {
    return {
      contents_title: 'Explore components',
      contents_url: 'https://vuetifyjs.com'
    }
  }
}
</script>
