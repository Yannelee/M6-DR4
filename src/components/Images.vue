<template>
  <div class="">
    <h2 class="titulo">{{title}}</h2>
    <div class="datos">
      <div class="img_div">
        <div v-for="(img, index) in imagesList" :key="img.src" @click="details(index)">
          <img :src="img.src" alt="" class="img">
        </div>
      </div>
      <div v-show="selected" class="detalles">
        <h3>{{imagesList[indexSelected].title}} ({{imagesList[indexSelected].year}})</h3>
        <img :src="imagesList[indexSelected].src" alt="">
        <p class="description">{{imagesList[indexSelected].descripcion}}</p>
        <button @click="cerrar" class="btnCerrar">Cerrar</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'images-component',
  props:{
    title:{
      type: String,
      default: 'Incubus Lists'
    },
    imagesList:{
      type: Array,
      require: true,
    },
  },
  data: function(){
    return{
      indexSelected: 0,
      selected: false
    }
  },
  methods:{
    details(index){
      this.indexSelected = index
      this.selected = true
    },
    cerrar(){
      this.selected = false
    }
  }
}
</script>

<style>
.titulo{
  margin: 0.2rem 2rem;
}
.datos{
  display: flex;
  justify-content: stretch;
  gap: 1rem;
  height: 93vh;
}
.img_div{
  overflow: auto;
  flex-basis: 30%;
}
.img{
  margin: .2rem;
  border-radius: .5rem;
  width: 95%;
}
.img:hover{
  cursor: pointer;
}
.detalles{
  margin: auto;
  text-align: center;
  flex-basis: 4;
  max-width: 50%;
  background-color: gainsboro;
  border-radius: .5rem;
  padding: 1rem;
}
.description{
  text-align: justify;
  max-height: 22rem;
  overflow: auto;
}
.btnCerrar{
  background-color: transparent;
  border: 1px solid silver;
  border-radius: .5rem;
  cursor: pointer;
  padding: .2rem 1rem;
  font-size: large;
}
.btnCerrar:hover{
  background-color: silver;
}
</style>