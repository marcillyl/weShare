<template>
  <div>
    <Header />
    <section class="home">
      <h1 class="home__headline">weShare</h1>
      <h2 class="home__text">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sunt illo ea
        aut quo, delectus officiis voluptatum vel corrupti deleniti quam nobis
        perspiciatis pariatur in sequi qui similique aspernatur quibusdam
        dolore?
      </h2>
      <NuxtLink to="/mountains" class="home__link"
        >Check out the mountains</NuxtLink
      >
    </section>
  </div>
</template>

<style>
.home {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.home__headline {
  font-size: 7em;
  font-weight: 300;
  color: aqua;
}
.home__text {
  max-width: 400pt;
  line-height: 1.7em;
  margin: 40pt;
}
.home__link {
  font-size: 1.4em;
}
</style>
