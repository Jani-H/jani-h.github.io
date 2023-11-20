<script>
  import { slide } from 'svelte/transition';
</script>

<main transition:slide>
  <div class="info-box">
    <h2>About me</h2>
    <p>
      I am 33 year old student and I currently live at Ainola, Jyväskylä. I
      study Business Information Technology at Jyväskylä University of Applied
      Sciences. I hope to specialize in programming and web design.
    </p>
  </div>
  <div class="info-box">
    <h2>This is me.</h2>
    <!-- svelte-ignore a11y-img-redundant-alt -->
    <img id="me" src="./images/me.png" alt="Picture of Me" />
  </div>
  <div class="info-box">
    <h2>Hobbies and Freetime</h2>
    <p>
      On my freetime I like playing video games with my friends, grilling at
      friends place and doing other things. I also enjoy traveling and seeing
      new places.
    </p>
  </div>
  <div class="info-box">
    <h2>Skills</h2>
    <h3>Languages</h3>
    <p>Finnish - Native Language</p>
    <p>English - Excellent</p>
  </div>
  <div class="info-box">
    <h2>Career</h2>
    <div>
      <h3>Saimaan Mediakeskus, full-time job 2018-2019</h3>
      <p>digi-assistant</p>
      <p>
        My job description included taking care of Lauritsala area’s schools
        information and communication related hardware.
      </p>
      <p>Job duration 8 months</p>
    </div>
    <div>
      <h3>Saimaan talous ja tieto Oy, summer job 2015</h3>
      <p>IT-support intern</p>
      <p>
        My job description included doing local and remote support, also phone
        support at a service point.
      </p>
      <p>Job duration 3 months</p>
    </div>
  </div>
  <div class="info-box">
    <h2>Education</h2>
    <div>
      <h3>Jyväskylä University of Applied Sciences, XX.XX.20XX</h3>
      <p>Tietojenkäsittely tradenomi tutkinto-ohjelma</p>
    </div>
    <div>
      <h3>Saimaan ammattiopisto Sampo, 31.03.2016</h3>
      <p>Tieto- ja viestintätekniikan perustutkinto</p>
    </div>
  </div>
</main>

<style>
  main {
    margin: 0em 15em;
    display: grid;
    grid-template-columns: 1fr 1fr;
    column-gap: 0.25em;
    row-gap: 0.25em;
    justify-content: center;
  }

  .info-box {
    margin: 0.25em;
    border-style: solid;
    border-color: black;
    border-width: 1px;
    border-radius: 5px;
    flex: 1;
    padding: 0.5em 0.5em;
    background-color: rgba(0, 0, 0, 0.5);
  }

  img {
    border-radius: 10px;
  }
</style>
