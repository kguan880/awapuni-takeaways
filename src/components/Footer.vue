<template>
  <div id="contact" class="footer">
    <div class="logo">
      Awapuni Takeaways
      <div class="hours">
        <br />
        <h4>Opening Hours:</h4>
        <p>
          Monday-Saturday: 11.30am - 1.30am | 4.30pm - 9pm <br />
          Sunday: 11.30am - 1.30am | 4.30pm - 8.30pm
        </p>
        <br />
      </div>
    </div>
    <div class="contact">
      <h2>Contact Us</h2>
      <br>
      <p>Phone: 06 354 1599</p>
      <p>40 Alexander Street, Palmerston North</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: space-around;
  background-color: midnightblue;
  height: 40vh;
  text-align: center;
  color: whitesmoke;
  align-items: center;
}

.hours {
  letter-spacing: 3px;
  font-size: 12px;
}
.footer .logo {
  display: flex;
  flex-direction: column;
  color: whitesmoke;
  text-transform: uppercase;
  letter-spacing: 7px;
  font-size: 30px;
  margin-top: 20px;
}

.footer .contact {
  letter-spacing: 3px;
}
</style>
