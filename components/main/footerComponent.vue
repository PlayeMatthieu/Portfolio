<template>
  <footer class="footer">
    <div class="content">
      <div class="columns is-centered">
        <div class="column is-4">
          <h2 class="title is-size-2">Interested in collaboration?</h2>
          <p class="subtitle">
            Feel free to send me an email. I’ll repond as soon as possible
          </p>
          <button class="button is-fullwidth">Let's Talk -></button>
        </div>
        <div class="column is-2">
          <ul>
            <li><a href="" class="title">Email</a></li>
            <li><a href="" class="title">Instagram</a></li>
            <li><a href="" class="title">Github</a></li>
            <li><a href="" class="title">Linkedin</a></li>
          </ul>
        </div>
      </div>
      <p class="has-text-centered">© 2021 Playe</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background: rgb(253, 251, 251);
  background: linear-gradient(
    50deg,
    rgba(253, 251, 251, 1) 0%,
    rgba(235, 237, 238, 1) 96%
  );
  padding: 3em 10em;
}

.button {
  background-color: #f5df84;
  color: #000;
  border-radius: 15px;
  padding: 1.5em 0;
  font-size: 22px;
  font-weight: 600;
}

ul li {
  list-style-type: none;
  font-size: 32px;
}

ul li a:hover {
  border-bottom: 5px solid #f5df84;
  transition: 2ms ease all;
}
</style>
