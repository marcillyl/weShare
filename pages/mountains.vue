<template>
  <div>
    <Header />
    <section class="list">
      <h1 class="list__headline">
        Mountains from <span class="list__headline--brand">Nuxt</span>
      </h1>
      <h2 class="list__text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab
        necessitatibus exercitationem laboriosam corporis beatae sit minus,
        nostrum ut dolorum. Et eligendi repudiandae quidem saepe tenetur
        officiis, maxime praesentium quam possimus?
      </h2>
      <p v-if="$fetchState.pending">Récupération des montagnes...</p>
      <p v-else-if="$fetchState.error">Une erreur est survenue :</p>
    </section>
    <main class="mountains">
      <article
        v-for="mountain of mountains"
        v-bind:key="mountain.id"
        class="mountain"
      >
        <NuxtLink :to="'/mountain/' + mountain.id" class="mountain__title"
          >{{ mountain.title }}
        </NuxtLink>
        <p>{{ mountain.height }}</p>
      </article>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mountains: [],
    };
  },
  async fetch() {
    this.mountains = await fetch("https://api.nuxtjs.dev/posts").then((res) =>
      res.json()
    );
  },
};
</script>

<style>
.list {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.list__headline {
  font-size: 4em;
  font-weight: 300;
  color: aqua;
}
.list__headline--brand {
  color: aqua;
}
.list__text {
  max-width: 400pt;
  line-height: 1.7em;
  margin: 40pt 0;
}
.mountains {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}
.mountain {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 14pt;
  width: 140pt;
  height: 140pt;
  border: solid thin white;
}
.mountain__title {
  margin-bottom: 14pt;
}
</style>
