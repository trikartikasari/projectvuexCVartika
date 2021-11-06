<template>
    
    <div class="row">
        <div class="a" style="background:palegoldenrod;">
            <h1 v-for="status in listData" :key="status">{{ status.judul }}</h1>
            <img src="https://www.kanalmu.com/ezoimgfmt/1.bp.blogspot.com/-9gnGRBguiDM/XkCluVx9XsI/AAAAAAAAANs/SF9_WhPOBzkyGF39bXjFcrn_rcehrNPCwCLcBGAsYHQ/s640/Gambar%2BKartun%2BMuslimah%2Bkanalmu.com%2B16.jpeg?ezimgfmt=rs:382x417/rscb2/ng:webp/ngcb2"><br><br>
            <h3 v-for="status in listData" :key="status">{{ status.judul1 }}</h3><hr><br><br>
            <p v-for="status in listData" :key="status"><span ><b>{{ status.alamat }}</b></span><br>
              {{ status.alamat2 }}<br>
            </p>
            <p v-for="status in listData" :key="status"><span><b>{{ status.phone }}</b></span><br>{{ status.phone2 }}</p>
            <p v-for="status in listData" :key="status"><span><b>{{ status.email }}</b></span><br>{{ status.email2 }}</p><br><br><br>
            <h3 v-for="status in listData" :key="status">{{ status.t }}</h3><hr><br>
            <h4 v-for="status in listData" :key="status">{{ status.j }}</h4>
            <h4 v-for="status in listData" :key="status">{{ status.k }}</h4>
            <h4 v-for="status in listData" :key="status">{{ status.l }}</h4>
            <br>
            <br>
            <h3 v-for="status in listData" :key="status">{{ status.u }}</h3><hr><br>
            <ul>
                <li v-for="status in listData" :key="status">{{ status.hobi }}</li>
                <li v-for="status in listData" :key="status">{{ status.hobi1 }}</li>
                <li v-for="status in listData" :key="status">{{ status.hobi2 }}</li>
            </ul>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
            <br>
        </div>
        <div class="a" style="background-color: brown">
            <h3 v-for="status in listData" :key="status">{{ status.v }}</h3><hr>
            <p v-for="status in listData" :key="status">{{ status.objek }}
            </p><br><br>
            <h3 v-for="status in listData" :key="status">{{ status.w }}</h3><hr>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;<sub v-for="status in listData" :key="status">{{ status.x }}</sub>
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
            <h3 v-for="status in listData" :key="status">{{ status.y }}</h3><hr>
            <p v-for="status in listData" :key="status">{{ status.education }}</p><br><br>
            <h3 v-for="status in listData" :key="status">{{ status.m }}</h3> <hr>
            <p v-for="status in listData" :key="status">{{ status.abiliti }}</p><br><br>
            <h3 v-for="status in listData" :key="status">{{ status.n }}</h3><hr>
            <p v-for="status in listData" :key="status">{{ status.pesan }}</p><br><br>
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
      width: auto;
      height: auto;
  }
  .row:after {
      border: 60px solid peachpuff;
  }
  h1 {
      color: olive;
  }
</style>