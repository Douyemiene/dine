<template>
  <main>
    <section class="section-one">
      <h2>dine</h2>
      <p class="thinHeading">Exquisite dining <br />since 1989</p>
      <p class="body-two text">
        Experience our seasonal menu in beautiful country surroundings. Eat the
        freshest produce from the comfort of our farmhouse.
      </p>
      <button class="button-transparent">book a table</button>
    </section>
    <section class="section-two">
      <Article
        :imageTop="true"
        image="homepage/enjoyable-place-mobile@2x.jpg"
        head=" Enjoyable place for all the family "
        text="Our relaxed surroundings make dining
      with us a great experience for everyone. We can even arrange a tour of the
      farm before your meal."
      />

      <div>
        <Article
          :imageTop="false"
          image="homepage/locally-sourced-mobile@2x.jpg"
          head="The most locally sourced food "
          text="All our ingredients come directly from our farm or local fishery. So you can be sure that you’re eating the freshest, most sustainable food."
        />
      </div>
    </section>
    <!-- section three -->
    <section>
      <div>
        <p class="highlight">
          A few highlights from our menu
        </p>
        <p class="body-two">
          We cater for all dietary requirements, but here’s a glimpse at some of
          our diner’s favourites. Our menu is revamped every season.
        </p>
      </div>
      <SmallArticle
        image="homepage/salmon-mobile@2x.jpg"
        head="Seared Salmon Fillet"
        text="Our locally sourced salmon served with a refreshing buckwheat summer salad."
      />
      <div id="verticalBorders">
        <SmallArticle
          image="homepage/beef-mobile@2x.jpg"
          head="Rosemary Filet Mignon "
          text="Our prime beef served to your taste with a delicious choice of seasonal sides."
        />
      </div>
      <SmallArticle
        image="homepage/chocolate-mobile@2x.jpg"
        head="Summer Fruit Chocolate Mousse"
        text="Creamy mousse combined with summer fruits and dark chocolate shavings."
      />
    </section>
    <!-- section four -->
    <section>
      <img
        src="./assets/homepage/family-gathering-mobile@2x.jpg"
        alt="family gathering"
      />
      <div>
        <div class="events">
          <h3 class="body-two">Family Ghering</h3>
          <h3 class="body-two">Special Events</h3>
          <h3 class="body-two">Social Events</h3>
        </div>
        <div>
          <p class="section-four-head">Family Gathering</p>
          <p class="body-two">
            We love catering for entire families. So please bring everyone along
            for a special meal with your loved ones. We’ll provide a memorable
            experience for all.
          </p>
          <button class="button-black">BOOK A TABLE</button>
        </div>
      </div>
    </section>
    <!-- section five -->
    <section>
      <h2>Ready to make a reservation?</h2>
      <button class="button-transparent">Book a table</button>
    </section>
  </main>
  <footer>
    <h2>dine</h2>
    <h4>
      Marthwaite, Sedbergh <br />
      Cumbria
    </h4>
    <h4></h4>
  </footer>
</template>

<script>
import Article from "./components/Article.vue";
import SmallArticle from "./components/SmallArticle.vue";
export default {
  name: "App",
  components: { Article, SmallArticle },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Spartan:wght@300;400;600;700&display=swap");

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  max-width: 100vw;
  font-family: "Spartan", sans-serif;
  font-size: 18px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: -0.22px;
}
main {
  position: relative;
}
.body-two {
  font-size: 15px;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: -0.19px;
}

.button-black {
  color: white;
  background: black;
  border: 1px solid white;
  width: 245px;
  height: 64px;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  text-transform: uppercase;
  padding: 1rem 2rem;
}

.button-transparent {
  color: white;
  border: 1px solid white;
  width: 245px;
  height: 64px;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: 1px;
  text-transform: uppercase;
  background: transparent;
  padding: 1rem 2rem;
}
h1 {
  font-size: 64px;
  font-weight: 300;
  line-height: 72px;
  letter-spacing: -0.8px;
}
h2 {
  font-size: 36px;
  line-height: 56px;
  letter-spacing: -0.5px;
}
h3 {
  font-size: 18px;
  font-weight: bold;
  line-height: 28px;
  letter-spacing: -0.22px;
}
h4 {
  font-size: 14px;
  font-weight: 500;
  line-height: 28px;
  letter-spacing: 2px;
}

.section-one {
  width: 100%;
  color: white;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 0 1.5rem;
  background-image: url("~@/assets/homepage/hero-bg-mobile@2x.jpg");
  background-position: center;
  background-size: cover;
}

.section-one h2:first-child {
  padding-top: 5rem;
  padding-bottom: 0.75rem;
}

.section-one .text {
  padding-bottom: 1.5rem;
}

.thinHeading {
  font-size: 32px;
  line-height: 40px;
  font-weight: 200;
  margin-bottom: 2rem;
  letter-spacing: 0.4px;
}

section:nth-child(3) {
  background: black;
  color: white;
  text-align: center;
  padding: 2rem 1rem;
}

section:nth-child(3) > div:first-child {
  padding: 0 1rem;
  padding-top: 3rem;
}

.highlight {
  font-size: 2rem;
  font-weight: 600;
  padding-bottom: 1rem;
}

#verticalBorders {
  border-top: 1px solid #979797;
  border-bottom: 1px solid #979797;
  margin: 0 1rem;
}

section:nth-child(4) {
  padding: 3rem 1.5rem;
  text-align: center;
}

section:nth-child(4) img {
  width: 100%;
  box-shadow: 1px solid black;
}

.events {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0.5rem 0;
}

.events h3 {
  font-weight: 500;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.section-four-head {
  font-size: 28px;
  font-weight: 600;
  text-align: center;
  padding: 1rem 0;
}

section:nth-child(5) {
  display: flex;
  flex-direction: column;
  justify-items: center;
  align-items: center;
  text-align: center;
  background-image: url("~@/assets/homepage/ready-bg-mobile@2x.jpg");
  color: white;
  padding: 2rem 0;
}

section:nth-child(5) > h2 {
  font-size: 32px;
}

footer {
  background: black;
  color: white;
  flex-direction: column;
  justify-items: center;
  text-align: center;
  padding: 2.5rem 0;
}

footer h4 {
  text-transform: uppercase;
}
</style>
