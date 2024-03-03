<template>
  <div class="container">
    <Nav />
    <Head />
    <Courses :data="courses" />
  </div>
</template>

<script>
import Nav from './components/Nav.vue';
import Head from './components/Head.vue';
import Courses from './components/Courses.vue';

export default {
  components: { Nav, Head, Courses },
  data() {
    return {
      courses: [
        {
          title: 'Кардио',
          cl: '250 калорий',
          time: '58:24',
          img: 'cardio.png',
        },
        {
          title: 'Растяжка',
          cl: '250 калорий',
          time: '58:24',
          img: 'stretch.png',
        },
        { title: 'Йога', cl: '250 калорий', time: '58:24', img: 'joga.png' },
        { title: 'Бег', cl: '250 калорий', time: '58:24', img: 'run.png' },
        {
          title: 'Гантели',
          cl: '250 калорий',
          time: '58:24',
          img: 'metal.png',
        },
        {
          title: 'На улице',
          cl: '250 калорий',
          time: '58:24',
          img: 'street.png',
        },
      ],
    };
  },
};
</script>

<style lang="scss">
$mainColor: #000000;
$textColor: #fff;
$additionColor: #25ab75;

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

::selection {
  background: #25ab75;
}

* {
  margin: 0;
  padding: 0;
}

body {
  background: $mainColor;
  color: $textColor;
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
}

a {
  color: #ababab;
  text-decoration: none;

  &:hover {
    color: #c7c7c7;
  }
}

.container {
  @media (min-width: 1500px) {
    width: 1300px;
    margin: 0 auto;
  }
  @media (max-width: 1500px) and (min-width: 900px) {
    width: 80%;
    margin: 0 10%;
  }
  @media (max-width: 900px) {
    width: 90%;
    margin: 0 5%;
  }
  @media (max-width: 900px) {
    width: 90%;
    margin: 0 5%;
  }
}
</style>
