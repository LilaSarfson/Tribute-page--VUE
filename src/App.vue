<script>
const PuccaData = [
  {
    id: 12,
    description:
      "Pucca (짜장소녀 뿌까, Jjajang Sonyeo Ppukka) is an animated comedy television series based on a series of shorts created by the South Korean company VOOZ Character System. The series revolves around Pucca, a young girl who is in love and obsessed with a ninja named Garu.",
  },
  {
    id: 13,
    description:
      "It also has aired on Champ TV and MBC TV in Korea. Internationally, series aired on Toon Disney's Jetix block in the United States,[1] Europe,[2] and other locales on the Jetix channel.[3] In Canada, the show aired on Family Channel.",
  },
  {
    id: 14,
    description:
      "Pucca premiered in 2006, with a set of 26 episodes (78 segments). Thesecond season of the show, consisting of 13 episodes (39 segments), began airing in 2008 after it was ordered to be created by Jetix Europe.",
  },
  {
    id: 15,
    description:
      "In October 2018, a third season was announced by Planeta Junior, a company within Planeta Group.[4]",
  },
  {
    id: 16,
    description:
      "The third season aired in South Korea on 10 December 2018 on MBC TV, segments).[6] The third season of Pucca, titled 'Pucca: Love Recipe' in English, released on Netflix on 31 December 2019.",
  },
  {
    id: 17,
    description:
      "In total, not including the previous online aired episodes of theshow, this brought the number of created segments to 191. The mains theme song is also sung in Korean.",
  },
];
import ImageComp from "./imageComp.vue";
import ListComp from "./DataPucca.vue";
export default {
  components: {
    ImageComp,
    ListComp,
  },
  data() {
    return {
      datosPucca: PuccaData,
    };
  },
};
</script>

<template>
  <main id="main">
    <img
      id="title"
      class="img-title"
      src="http://assets.stickpng.com/thumbs/5a9c10219fc609199d0ff07b.png"
      alt="PUCCA"
    />

    <h2>UN AMOR QUE TE DEJARÁ SIN PALABRAS</h2>
    <ImageComp
      legend="Pucca and Garu"
      urlImage="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSU5WfKEyTb_BHsW8NNky3PmQiS0FpAVFG0bg&usqp=CAU"
    />
    <div id="tribute-info">
      <h2 style="color: black">Here's the Pucca Show life</h2>
      <ListComp :items="datosPucca" />
    </div>
    <footer>
      <a
        target="_blank"
        id="tribute-link"
        href="https://en.wikipedia.org/wiki/Pucca_(TV_series)"
        >More information about PUCCA
      </a>
    </footer>
  </main>
</template>

<style>
@import "./assets/base.css";

#main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
#title {
  font-size: 5rem;
  color: black;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
#tribute-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  background-color: rgb(253, 215, 215);
}
.img-title {
  width: 200px;
  align-items: center;
}
footer {
  margin-top: 2rem;
  text-align: center;
  justify-items: center;
}
h2 {
  color: black;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
a {
  margin-top: 0;
  text-decoration: none;
  color: hsla(160, 100%, 37%, 1);
  transition: 0.4s;
  font-weight: bold;
}

@media (min-width: 1024px) {
  body {
    display: flex;
  }

  header {
    display: flex;
    padding-right: calc(var(--section-gap) / 2);
  }
}
</style>
