<template>
  <div class="home-component">
    <home-item v-for="photoLogsData in arrayOfPhotoLogs" :key="photoLogsData" :photoLogsData="photoLogsData">
    </home-item>
  </div>
</template>

<script>
import HomeItem from "../components/HomeItem.vue";
export default {
  data() {
    return {
      arrayOfPhotoLogs: [],
    }
  },
  components: {
    HomeItem,
  },
  methods: {
    async getPhotoLogs() {
      const response = await fetch("http://localhost:3000/photo-logs/")
      const data = await response.json(); // response는 json데이터이고, 그것을 data라는 변수로 지정해줌
      this.arrayOfPhotoLogs = data.photoLogsData; // 그 데이터 안에 있는 photoLogsData를 비어있는 arrayOfPhotoLogs에 넣어줌
    }
    // async: function이 끝나기 전까지는 어떤 것도 실행하지 않고 기다림
    // fetch: "http://localhost3000:photo-logs/" 서버로부터 데이터를 가지고 옴
    // 서버로부터 가지고 올 데이터가 많은 경우에는, 가지고 오는 도중에 실행이 되지 않도록 모든 데이터들을 다 가지고 온 다음에 실행이 되도록 기다리는 것임
  },
  // Vue의 LifeCycle중에 mounted()를 해주면, 홈페이지 메인화면에 들어가자마자 getPhotoLogs라는 function이 실행되게 해줌
  mounted() {
    this.getPhotoLogs();
  },
}
</script>

<style scoped>
.home-component {
  display: flex;
}
</style>