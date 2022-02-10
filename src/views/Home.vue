<template>
  <div class="home">
    <h1>Цветотип Внешности</h1>
    <h2>распространённая классификация цветотипов по временам года</h2>
    <section class="all-types">
      <a href="" class="season-link main-link summer"
        ><span class="underline">лето</span>
      </a>
      <a href="" class="season-link main-link spring">весна</a>
      <img
        src="../assets/img/circle.png"
        alt="circle color types apperience"
        width="700"
      />
      <a href="" class="season-link main-link autumn">осень</a>
      <a href="" class="season-link main-link winter">зима</a>
    </section>

    <div class="description-row">
      <p>
        Существует 4 глобальных цветотипа. Каждый из 4 цветотипов разделяется
        еще на 3 подтипа. Таким образом, всего существует 12 цветотипов
        внешности. Каждый из них обладает своими уникальными характеристиками.
      </p>
      <p>
        Цветотип зависит от оттенков волос, кожи, глаз. Вместе они создают общий
        фон, который может гармонировать с другими окружающими расцветками. Или,
        напротив, диссонировать.
      </p>
    </div>
    <button class="btn">узнать свой цветотип</button>
  </div>

  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: "Home",
  components: {
    // HelloWorld
  },
};
</script>

<style scoped>
h1 {
  color: #b87c7c;
}

.all-types {
  margin: 3rem auto;
  width: 80vw;
  display: flex;
  justify-content: center;
}

.summer,
.autumn {
  align-self: flex-start;
  align-content: flex-start;
}
.spring,
.winter {
  align-self: flex-end;
}

.description-row {
  display: flex;
  justify-content: center;
}
.description-row {
  text-align: left;
}

.description-row p {
  width: 36vw;
  margin: 1rem 2rem;
}

.season-link {
  text-decoration: none;
  /* text-decoration: underline;
  text-decoration-thickness: 12px;
  text-decoration-color: #ebdbbf;
  text-underline-position: under; */
}
.main-link {
  font-size: 1.5em;
  line-height: 1.6;
  color: rgba(133, 117, 97, 0.7);
}

.underline {
  text-decoration: none;
  position: relative;
  padding: 0 0.5rem;
  transition: 1s ease;
  border-radius: 2px;
}
.underline:after {
  content: "";
  width: 100%;
  height: 1rem;
  margin: 0 auto;
  position: absolute;
  left: 0;
  right: 0;
  left: 0;
  background-color: #ebdbbf7c;
  bottom: -0.4rem;
  border-radius: 2px;
}
.underline:hover {
  background-color: #ebdbbf9c;
}
</style>