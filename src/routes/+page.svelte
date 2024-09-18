<script>
  export let data;
</script>

<div class="container">
  <div class="profile">
    <!-- Avatar en informatie -->
    <!-- <div class="avatar">
        <img src="{data.person.avatar}" alt="Annelinde"/>
    </div> -->

    <section class="info-text">
      <h1>{data.person.name} {data.person.surname}</h1>
      <h2 class="intro">Hi There! I’m a <span>front-end developer</span></h2>
      <p>{data.person.bio}</p>
    </section>

    <!-- Skills sectie -->
    <section class="skills">
      <h2>My Skills</h2>
      <div class="skill skill-html">
        <h3>HTML</h3>
        <p>Creating websites with structure.</p>
      </div>
      <div class="skill skill-css">
        <h3>CSS</h3>
        <p>Styling websites to look great.</p>
      </div>
      <div class="skill skill-js">
        <h3>JavaScript</h3>
        <p>Making websites interactive and dynamic.</p>
      </div>
      <div class="skill skill-github">
        <h3>GitHub</h3>
        <p>Collaborating on code projects.</p>
      </div>
      <div class="skill skill-svelte">
        <h3>Svelte</h3>
        <p>Building fast, reactive websites with minimal code.</p>
      </div>
    </section>

    <!-- Social media links -->
    <section class="socials">
      <a href="https://www.instagram.com/annelinde.r/" target="_blank" class="btn">
        <i class="fa-brands fa-instagram"></i>
        <p>Instagram</p>
      </a>
      <a href="https://github.com/annelinderaadsheer?tab=repositories" target="_blank" class="btn">
        <i class="fa-brands fa-github"></i>
        <p>Github</p>
      </a>
      <a href="https://www.linkedin.com/in/annelinde-raadsheer-b38375194/" target="_blank" class="btn">
        <i class="fa-brands fa-linkedin"></i>
        <p>Linked-in</p>
      </a>
    </section>
  </div>
</div>

<style>
  * {
    margin: 0;
    padding: 0;
    font-family: 'Georgia', serif;
    box-sizing: border-box;
  }

  .container {
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #BBA58F, #E8D9CD);
  }

  .profile {
    width: 90%;
    max-width: 450px;
    background: linear-gradient(145deg, #BBA58F, #523D35);
    text-align: center;
    padding: 30px 20px;
    box-shadow: 0 10px 60px rgba(0, 0, 0, 0.2);
    border-radius: 20px;
    transition: transform 0.3s ease;
  }

  .profile:hover {
    transform: translateY(-10px);
  }

  .info-text {
    margin-top: 20px;
    color: #FFFFFF;
  }

  .info-text h1 {
    font-size: 2em;
    font-weight: 700;
    margin-bottom: 10px;
    color: #ffffff;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  }

  .info-text h2.intro {
    font-size: 1.2em;
    margin-bottom: 20px;
    color: #ffffff;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.4);
    white-space: nowrap;
    overflow: hidden;
    border-right: 2px solid #ffffff;
    animation: typing 4s steps(40, end), blink-caret 0.75s step-end infinite;
  }

  .info-text h2.intro span {
    color: #523D35;
    font-weight: bold;
  }

  .info-text p {
    font-size: 1em;
    line-height: 1.5;
    color: #f0f0f0;
  }

  .skills {
    margin-top: 30px;
  }

  .skills h2 {
    text-align: center;
    margin-bottom: 20px;
    color: #523D35;
    font-size: 1.2em;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.4);
  }

  .skill {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    padding: 10px;
    margin-bottom: 15px;
    position: relative;
    overflow: hidden;
  }

  .skill h3 {
    font-size: 1.2em;
    color: #ffffff;
    margin-bottom: 5px;
  }

  .skill p {
    font-size: 0.9em;
    color: #f0f0f0;
  }

  /* Gradient hover effect */
  .skill::before {
    content: "";
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, #BBA58F, #523D35);
    transition: left 0.5s ease;
    z-index: 0;
  }

  .skill:hover::before {
    left: 0;
  }

  .skill h3, .skill p {
    position: relative;
    z-index: 1;
  }

  /* Breedtes for skills */
  .skill-html::before {
    width: 100%;
  }

  .skill-css::before {
    width: 66.67%;
  }

  .skill-js::before {
    width: 33.33%;
  }

  .skill-github::before {
    width: 66.67%;
  }

  .skill-svelte::before {
    width: 66.67%;
  }

  /* Type animatie */
  @keyframes typing {
    from { width: 0; }
    to { width: 100%; }
  }

  @keyframes blink-caret {
    from, to { border-color: transparent; }
    50% { border-color: #ffffff; }
  }

  .btn {
    text-decoration: none;
    color: rgba(0, 0, 0, 0.5);
    padding: 10px 10px;
    border-radius: 8px;
    display: inline-block;
    margin: 40px 0;
    transition: transform 0.3s ease-in-out;
  }

  .btn:hover {
    transform: translateY(-10px);
  }
</style>