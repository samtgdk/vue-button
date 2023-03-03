<template>
  <div class="window">

    <h1>sayim:{{sayi}}</h1>
    <div class="d-flex gap-2">
       <button @click="arttir(5)" class="btn btn-success">Arttır</button>
       <button @click="azalt(2)" class="btn btn-danger">Azalt</button>
    </div>
   
  </div>
</template>

<script>




export default{

  name:'app',
  data() {
    return {
      isim:'MERT',
      soyisim:'ulusoy',
      yas:20,
      a:10,
      sayi:0,
    }
  },
  methods: {
    arttir(kackac){
      this.sayi = this.sayi +kackac;
    },
    azalt(kackac){
      this.sayi = this.sayi - kackac;
    }
  },
  mounted() {
    
  },
   
}



</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.window{
  width: 100%;
  margin-top: 25px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
