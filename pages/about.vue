<template>
  <main class="container">
    <section class="">
      <div class="about-page-content">
        <h1>Hello</h1>
        <img
          src="~/assets/img/about_me-min.png"
          alt="Matthieu"
          loading="lazy"
        />
      </div>
      <p>
        My name is <b>Matthieu Playe</b>, and I’m a student in software
        development from Belgium. I am currently working in a roofing company as
        a calculator.
      </p>
      <p>
        By developing software I help myself and other people by making their
        work easier.
      </p>
      <p>
        In my spare time, I like to learn more about design and programming, I
        enjoy listening to music and quality time with family.
      </p>
    </section>
  </main>
</template>

<style scoped>
.about-page-content {
  position: relative;
  margin-top: 6em;
  height: 30vh;
  width: 100%;
  display: flex;
  align-content: center;
  margin-bottom: 2em;
}
h1 {
  z-index: 10;
  font-size: 20vw;
}
p {
  margin: 15px 0;
}
img {
  position: absolute;
  right: 0;
  top: 0;
  height: 100%;
  max-height: 30vh;
}
@media (min-width: 768px) {
  .about-page-content {
    height: 40vh;
    width: 100%;
    margin-top: 0;
    margin-bottom: 4em;
  }
  h1 {
    z-index: 10;
    font-size: 25vw;
  }
  img {
    height: 100%;
    max-height: 40vh;
  }
}
@media (min-width: 1200px) {
  .about-page-content {
    height: 50vh;
    width: 100%;
    margin-bottom: 5em;
  }
  h1 {
    z-index: 10;
    font-size: 20em;
  }
  img {
    height: 100%;
    max-height: 60vh;
  }
}
</style>
