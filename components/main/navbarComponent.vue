<template>
  <div class="container">
    <b-navbar>
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <h2 class="title">Playe.be</h2>
        </b-navbar-item>
      </template>
      <template #end>
        <b-navbar-item href="#"> Home </b-navbar-item>
        <b-navbar-item href="#"> About </b-navbar-item>
        <b-navbar-item href="#"> Contact </b-navbar-item>
      </template>
    </b-navbar>
  </div>
</template>
