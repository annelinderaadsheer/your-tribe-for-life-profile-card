<h1>Hello world</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<!-- ProfileCard.svelte -->
<style>
  * {
    margin: 0;
    padding: 0;
    font-family: Georgia, serif;
    box-sizing: border-box;
  }

  .container {
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(#BBA58F, #E8D9CD);
  }

  .profile {
    width: 90%;
    max-width: 320px;
    background: linear-gradient(#BBA58F, #523D35);
    text-align: center;
    padding: 30px 20px;
    box-shadow: 0 10px 140px rgba(0, 0, 0, 0.2);
    border: 3px solid #ffffff;
    border-radius: 20px;
  }

  .profile h1 {
    font-size: 16px;
    color: #ffffff;
  }

  h1 span {
    color: #523D35;
  }

  .skills h2 {
    text-align: center;
    margin-bottom: 20px;
    color: #523D35;
    font-size: 18px;
  }

  .skill {
    text-align: center;
    margin-bottom: 20px;
  }

  .skill h3 {
    font-size: 16px;
    color: #ffffff;
  }

  .skill p {
    font-size: 14px;
    color: #ffffff;
  }
</style>

<div class="container">
  <div class="profile">
    <h1>Hi There! My name is Annelinde and I’m a <span>front-end developer</span></h1>

    <!-- Skills -->
    <div class="skills">
      <h2>My Skills</h2>
      <div class="skill">
        <h3>HTML</h3>
        <p>Creating websites with structure.</p>
      </div>
      <div class="skill">
        <h3>CSS</h3>
        <p>Styling websites to look great.</p>
      </div>
      <div class="skill">
        <h3>JavaScript</h3>
        <p>Making websites interactive and dynamic.</p>
      </div>
      <div class="skill">
        <h3>GitHub</h3>
        <p>Collaborating on code projects.</p>
      </div>
      <div class="skill">
        <h3>NPM</h3>
        <p>Managing and installing packages.</p>
      </div>
    </div>
  </div>
</div>