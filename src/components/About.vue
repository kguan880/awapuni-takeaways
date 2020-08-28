<template>
  <div id="about">
    <div class="container-row">
      <div class="image-box">
        <img src="@/assets/mum.jpg" alt="" />
      </div>
      <div class="text-box">
        <h1>About Us</h1>
        <p class="summary">
          Welcome to Awapuni Takeaways, Palmerston North's number one fish and
          chip shop ! <br />
          <br />
          My name is Elaine and my husband and I have been running this shop for
          almost 25 years. We have 3 grown children who many of my customers
          have seen since they were little kids. They are all doing there own
          things now but they still come in to help their mum and dad when the
          shop gets busy, especially on fridays ! <br />
          I love talking with my customers and learning about them. I know all
          my regular customers faces, names, and what they love to order every
          time. If you are new, I will do my best to introduce myself and learn
          more about you too. <br /><br />
          We guarantee that we have the best prices in all of Palmerston North
          and the most tasty fish and chips you can find. <br /><br />
        </p>
        <h3>Check out our menu below !</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
#about {
  align-items: center;
  display: flex;
  justify-content: center;
}

.text-box {
  width: 60%;
  height: 80vh;
  padding: 10px 10px 0px 50px;
  font-size: 1em;
}

.image-box {
  width: 30%;
  height: 80vh;
  padding: 10px 0px 0px 100px;
}

.image-box img {
  height: 500px;
  width: 300px;
}

@media screen and (max-width: 768px) {
  .image-box {
    display: none;
  }

  .text-box {
    width: 100%;
    font-size: 1.5em;
  }
}
</style>
