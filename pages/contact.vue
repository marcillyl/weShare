<template>
  <div>
    <Header />
    <section class="contact">
      <h1 class="contact__headline">Let's talk</h1>
      <h2 class="contact__text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab
        necessitatibus exercitationem laboriosam corporis beatae sit minus,
        nostrum ut dolorum. Et eligendi repudiandae quidem saepe tenetur
        officiis, maxime praesentium quam possimus?
      </h2>
    </section>
  </div>
</template>

<style>
.contact {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.contact__headline {
  font-size: 7em;
  font-weight: 300;
  color: aqua;
}
.contact__text {
  max-width: 400pt;
  line-height: 1.7em;
  margin: 40pt 0;
}
</style>
