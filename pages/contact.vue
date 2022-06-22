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
    <form action="" class="form">
      <input type="text" class="form__input" placeholder="Name" />
      <input type="email" class="form__input" placeholder="Email" />
      <textarea
        name="message"
        id="message"
        cols="30"
        rows="10"
        class="form__input"
        placeholder="Message"
      ></textarea>
      <button type="submit" class="form__button">Send</button>
    </form>
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
.form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.form__input {
  width: 30em;
  padding: 4pt;
  margin: 7pt;
  background: #111;
  border: solid thin #222;
}
.form__button {
  padding: 4pt 7pt;
  border: solid thin aqua;
  color: aqua;
  margin: 10pt;
}
</style>
