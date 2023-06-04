<template>
  <div id="app">
    <Images :imagesList="imgList" :title="title" class="images"/>
  </div>
</template>

<script>
import Images from "@/components/Images.vue"

export default {
  name: 'App',
  components: {
    Images
  },
  data: function(){
    return{
      title: 'Discografía Incubus',
      imgList: [
        {
          src:"https://upload.wikimedia.org/wikipedia/en/9/92/Fungus_amongus.jpg", 
          title: 'Fungus Amongus',
          year: 1995,
          descripcion: 'Primer álbum de estudio de la banda estadounidense de funk metal Incubus, publicado el 1 de noviembre de 1995 bajo su propio sello discográfico independiente llamado Stopuglynailfungus Music On Chillum. Brandon Boyd rememora sobre las grabaciones iniciales, notando el material del álbum como una producción jovial, influenciado por distintas bandas como Led Zeppelin y The Doors, aspectos funk metal de Primus, Mr. Bungle y Faith No More, como también bandas del movimiento grunge: Pearl Jam, Soundgarden, Nirvana y Alice in Chains; esto cuando tenían alrededor de 15 años.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/4/4f/Incubus_Science.jpg", 
          title: 'S.C.I.E.N.C.E',
          year: 1997,
          descripcion: `Segundo álbum de estudio de la banda, lanzado al mercado el 9 de septiembre de 1997. El disco trae el vídeo de "A Certain Shade of Green". El álbum hasta la fecha ha vendido más de 750.000 copias en Estados Unidos. Contiene algo del trabajo más pesado de la banda y es considerado por muchos fanáticos como la definición original de su sonido. Es una fusión de varias influencias con características de sus tendencias experimentales. No es un indicativo de su siguiente álbum Make Yourself, el cual es referido en varias reseñas como el punto máximo de interpretación de la banda.El álbum combina Rock, Thrash Metal, Funk, Hip Hop, Jazz y Techno. S.C.I.E.N.C.E. fue nombrado así porque la banda sintió que estaban trabajando en un proyecto de ciencias mientras creaban el disco, como tal, el acrónimo S.C.I.E.N.C.E. no tiene un significado real, en lugar de eso la banda escogió en dejar a la gente interpretarlo de la forma en que ellos lo ven. El acrónimo es un enigma al igual que el hombre del bigote de la portada. La banda ha dado significados contradictorios tanto para el nombre del álbum y la cara de "Chuck" cuya imagen también aparece en el Enjoy Incubus EP. Se ha especulado también que la cara de la portada es la de su maestro de ciencias del 8º grado quien los inspiró. Algunos de los significados de S.C.I.E.N.C.E. son los siguientes: 'Sailing Catamarans Is Every Nautical Captain's Ecstasy'; 'Smoke Cannabis It Exists Naturally Credit Earth'; 'Southern California's Incubus Enters Nevada Carrying Enstruments'; 'Social Chronology Includes Everyone: Neanderthals, Cannibals, Everyone'.`
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/b/ba/Incubus_make_yourself.jpg", 
          title: 'Make Yourself',
          year: 1999,
          descripcion: 'Tercer álbum de estudio de la banda, lanzado el 26 de octubre de 1999. A menudo es considerado el mejor álbum de la banda hasta la fecha. Ha sido certificado como disco de platino en Estados Unidos. El disco trae los hits Pardon Me, Stellar y el tema con el que se dieron a conocer a todos que es Drive, los cuales llegaron a estar entre los 3 primeros lugares de la Billboard. Para muchos fanáticos Make Yourself representa un cambio de sonido significativo de la banda, con una mayor calidad en la producción musical y con un sonido más maduro que su anterior álbum S.C.I.E.N.C.E. De alguna manera Make Yourself es un avance de su álbum Morning View, el más popular de todos. Este es el primer álbum que se grabó con DJ Kilmore quien reemplazó a DJ Lyfe.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/6/68/Incubus_-_Morning_View.jpg", 
          title: 'Morning View',
          year: 2001,
          descripcion: 'Cuarto álbum de la banda, publicado por Epic Records el 23 de octubre de 2001. Este fue el último álbum en contar con el bajista Alex Katunich, dejando la banda a comienzos de 2003 por diferencias personales. Una grabación más positiva y liberadora que sus anteriores trabajos, refleja el ambiente que se respiraba en el estudio de grabación situado en la calle que da nombre al disco.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/8/8d/ACrowLeftoftheMurderIncubus.jpg", 
          title: 'A Crow left of the Murder...',
          year: 2004,
          descripcion: 'Quinto álbum de la banda, publicado el 3 de febrero de 2004. Es el primer disco donde sale el nuevo bajista Ben Kenney, quien reemplaza a Dirk Lance.Los singles de este álbum fueron "Megalomaniac" y "Talk Shows on Mute". "Agoraphobia" y "Sick Sad Little World" fueron también lanzados como singles solo para las emisoras; como consecuencia, solo las canciones "Megalomaniac" y "Talk shows on Mute" tuvieron videos musicales o videoclips. El álbum debutó en el puesto #2 en los U.S. Billboard 200, vendiendo cerca de 332 000 copias en su primera semana. Desde entonces se han vendido aproximadamente 1,5 millones de copias.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/0/0f/Incubus_-_Light_Grenades.jpg", 
          title: 'Light Grenades',
          year: 2006,
          descripcion: 'Sexto álbum de la banda, anzado el 28 de noviembre de 2006. El álbum vendió en su primera semana 229 000 copias alrededor del mundo, la mayoría en los EE. UU. El álbum debutó en el #1 de la Billboard 200, vendiendo en los EE. UU. 165 000 copias. Sin embargo, Light Greandes tiene el triste récord de la mayor caída de un álbum debut en el #1 de la lista, cayendo de la posición #1 a la #37 en su segunda semana en la Billboard 200, superando el récord de Marilyn Manson y su álbum The Golden Age of Grotesque que cayó del #1 al #21 en el año 2003. Hoy el álbum ha obtenido Disco de Oro en EE. UU. y hasta la fecha ha vendido 700 000 en EE. UU.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/2/22/If_not_now_when_album_cover.jpg", 
          title: 'If not Now, When?',
          year: 2011,
          descripcion: 'Séptimo álbum de la banda, lanzado el 12 de julio de 2011. El primer sencillo del álbum es Adolescents. Existen 3 caras B de este último trabajo, no incluidas en el álbum: Surface to air, Rebel girls y Hold me down.'
        },
        {
          src:"https://upload.wikimedia.org/wikipedia/en/c/ce/Incubus_8_Artwork.jpg", 
          title: '8',
          year: 2017,
          descripcion: 'Octavo álbum la banda, lanzado el 21 de abril de 2017. Es el primer álbum de estudio de la banda desde If Not Now, When? y el primer álbum que se lanzará a partir de Island Records. El primer sencillo «Nimble Bastard» fue lanzado el 16 de febrero de 2017.'
        }
      ]
    }
  },
}
</script>

<style>
#app{
  height: 98vh;
  border: 1px solid silver;
  background-color: whitesmoke;
  border-radius: 1rem;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  padding: 0 1rem;
}
</style>
