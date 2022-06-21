<template>
  <Home />
</template>

<script>
export default {
  name: "IndexPage",
};
</script>

<style>
@font-face {
  font-family: "MontserratAlternates";
  src: url("./assets/Fonts/Montserrat_Alternates/MontserratAlternates-Regular.ttf")
    format("truetype");
  font-weight: 400;
}
@font-face {
  font-family: "MontserratAlternates";
  src: url("./assets/Fonts/Montserrat_Alternates/MontserratAlternates-Light.ttf")
    format("truetype");
  font-weight: 300;
}
*,
*::before,
*::after {
  box-sizing: inherit;
  margin: 0;
}
html {
  box-sizing: border-box;
  scroll-behavior: smooth;
  min-width: 320px;
}
body {
  font-family: "MontserratAlternates", Arial, Helvetica, sans-serif;
  background: #171717;
  color: #fff;
  font-size: 14px;
}
img {
  object-fit: cover;
}
a {
  cursor: pointer;
  color: #fff;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: 1em;
  font-weight: 400;
}
button,
button::before,
button::after {
  cursor: pointer;
  font-family: "MontserratAlternates", Arial, Helvetica, sans-serif;
  border: none;
  background: transparent;
  color: #fff;
  font-size: 1em;
  font-weight: 400;
}
input,
input::before,
input::after,
textarea,
textarea::before,
textarea::after {
  font-family: "MontserratAlternates", Arial, Helvetica, sans-serif;
  border: none;
  resize: none;
  color: #fff;
  font-size: 1em;
  font-weight: 400;
}
ul,
ul::before,
ul::after,
li,
li::before,
li::after {
  display: flex;
  justify-content: space-between;
  align-items: center;
  list-style-type: none;
  padding: 0;
}
</style>
