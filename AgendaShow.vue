<template>
<div class="row">
<div class="a" style="background-color: olive">
    <img src="https://i.pinimg.com/originals/a1/b8/ef/a1b8ef1ce80033bd1afd125c3e2cd9a4.jpg">
<h3 v-for="status in listData" :key="status" >{{ status.ab }}</h3><hr style="border-top: dashed 1px;" />
 <p v-for="status in listData" :key="status"><span><b>{{ status.ab2 }}</b></span><br>{{ status.ab7 }}</p><br>
 <p v-for="status in listData" :key="status"><span><b>{{ status.ab3 }}</b></span><br>{{ status.ab8 }}</p><br>
 <p v-for="status in listData" :key="status"><span><b>{{ status.ab4 }}</b></span><br>
 {{ status.ab9 }}<br>{{ status.b2 }}</p><br><br>
 <p v-for="status in listData" :key="status"><span><b>{{ status.ab5 }}</b></span><br>{{ status.b3 }}</p><br>
 <p v-for="status in listData" :key="status"><span><b>{{ status.ab6 }}</b></span><br>{{ status.b4 }}</p><br>
<h3 v-for="status in listData" :key="status">{{ status.r }}</h3><hr style="border-top: dashed 1px;" ><br>
            <ul>
                <li v-for="status in listData" :key="status">{{ status.hobi }}</li>
                <li v-for="status in listData" :key="status">{{ status.hobi1 }}</li>
                <li v-for="status in listData" :key="status">{{ status.hobi2 }}</li>
            </ul>
            <br>
<h3 v-for="status in listData" :key="status">{{ status.q }}</h3><hr style="border-top: dashed 1px;" />
<p v-for="status in listData" :key="status">{{ status.p }}
</p><br>
<h3 v-for="status in listData" :key="status">{{ status.ape }}</h3><hr style="border-top: dashed 1px;" />
<p v-for="status in listData" :key="status">{{ status.b5 }}
</p><br>
</div>
<div class="a" style="background-color: darkolivegreen">
    <h1 v-for="status in listData" :key="status">{{ status.nama }}</h1>
    <h2 v-for="status in listData" :key="status">{{ status.apa }}</h2><hr style="border: 1px solid black;">
    <div class="b" style="background-color: grey;">
            <h3 v-for="status in listData" :key="status">&#127773;{{ status.w }}</h3><hr style="border-top: dashed 1px;" />
            <p v-for="status in listData" :key="status">{{ status.hidup }}<br>
                <ul>
                    <li v-for="status in listData" :key="status">{{ status.a }}</li>
                    <li v-for="status in listData" :key="status">{{ status.b }}</li>
                    <li v-for="status in listData" :key="status">{{ status.c }}</li>
                    <li v-for="status in listData" :key="status">{{ status.d }}</li>
                    <li v-for="status in listData" :key="status">{{ status.e }}</li>
                    <li v-for="status in listData" :key="status">{{ status.f }}</li>
                    <li v-for="status in listData" :key="status">{{ status.g }}</li>

                </ul></p><br><br>
    </div>
    <div class="b"  style="background-color: grey;">
            <h3 v-for="status in listData" :key="status">&#x1F341;{{ status.n }}</h3><hr>
            <p v-for="status in listData" :key="status">{{ status.pesan }}</p><br><br>
    </div>
</div>

</div>
</template>
<script>
export default {
    name: 'AgendaShow',
    computed: {
      
        listData() {
            return this.$store.state.listData;
        },
    }
}
</script>
<style scoped>

* {
    box-sizing: border-box;
  }
  
  /* Create four equal columns that floats next to each other */
  .a {
    float: left;
    width: 40%;
    padding: 50px;
  }
  
  /* Clear floats after the columns */
  .row:after {
    content: "";
    display: table;
    clear: both;
  }
  
  /* Responsive layout - makes a two column-layout instead of four columns */
  @media screen and (max-width: 500px) {
    .a  {
      width: 40%;
    }
  }
  
  /* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
  @media screen and (max-width: 500px) {
    .a {
      width: 40%;
    }
  }
  img {
      width: 300px;
      height: 450px;
  }
  .row:after{
      border: 60px solid darkkhaki;
  }
</style>