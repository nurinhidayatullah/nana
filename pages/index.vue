<template>
  <div class="content">
    <div v-if="pageIndex == 0" class="card shadow" style="background-color: black;">
      <div class="card-body" style="background-color: black;">
        <button  class="btn btn-primary btn-lg" @click="pageIndex=1">Tekan Disini</button>
      </div>
    </div>
    <div v-if="pageIndex == 1" class="card">
      <div class="card-body">
        <h4>Tinggal Klik Klik Lanjut Jak</h4><br>
        <button  class="btn btn-primary btn-lg" @click="pageIndex=2">Lanjut</button>
      </div>
    </div>
    <div v-if="pageIndex == 2" class="card">
      <div class="card-body">
        <img src="@/assets/1.jpg" class="img img-fluid" alt="">
        <h4>NGESELIN</h4><br>
        <button  class="btn btn-primary btn-lg" @click="pageIndex=3">Lanjut</button>
      </div>
    </div>
    <div v-if="pageIndex == 3" class="card">
      <div class="card-body">
        <img src="@/assets/2.jpg" class="img img-fluid" alt="">
        <h4>CUEK</h4><br>
        <button  class="btn btn-primary btn-lg" @click="pageIndex=4">Lanjut</button>
      </div>
    </div>
    <div v-if="pageIndex == 4" class="card">
      <div class="card-body">
        <img src="@/assets/gif.gif" class="img img-fluid" alt="">
        <h4>TAPI SAYANG AKU TUH SAME DIE!!!</h4><br>
        <button  class="btn btn-primary btn-lg" @click="pageIndex=0">Ulang</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      pageIndex: 0
    }
  },
  mounted() {
    this.pageIndex = 0;
  }
};
</script>
