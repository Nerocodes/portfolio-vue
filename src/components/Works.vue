<template>
  <section class="works">
    <button class="works-btn" @click="toggleWorks">View my works</button>
    <div class="sites">
      <div class="site hide">
        <p class="title">Wedeydo</p>
        <p class="description">Crowdfunding apllication</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            React
          </details>
          <details>
            <summary>Backend</summary>
            Nodejs <br>
            Postgresql
          </details>
        </details>
        <a href="https://wedeydo.com" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site">
        <p class="title">Temitope Odushola</p>
        <p class="description">Music personality</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Vanilla JavaScript
          </details>
        </details>
        <a href="https://brave-rosalind-140a13.netlify.app/" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site">
        <p class="title">Teelonis</p>
        <p class="description">All about gifts</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Nuxtjs, Vuejs
          </details>
        </details>
        <a href="https://superlative-duckanoo-4ac339.netlify.app/" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site">
        <p class="title">OviePaulEj</p>
        <p class="description">Portfolio</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Wordpress
          </details>
          <details>
            <summary>Backend</summary>
            PHP <br>
            MySQL
          </details>
        </details>
        <a href="https://oviepaulej.com/" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site">
        <p class="title">Banka</p>
        <p class="description">banking application</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Vanilla JavaScript
          </details>
          <details>
            <summary>Backend</summary>
            Nodejs <br>
            Postgresql
          </details>
        </details>
        <a href="https://nerocodes.github.io/banka/ui/" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site hide">
        <p class="title">Hannah Ephraim</p>
        <p class="description">Jewellery store</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Wordpress
          </details>
          <details>
            <summary>Backend</summary>
            PHP <br>
            MySQL
          </details>
        </details>
        <a href="https://hannahephraim.com/" class="visit-btn" target="blank">View app</a>
      </div>
      <div class="site">
        <p class="title">Farmly</p>
        <p class="description">Farming Automation</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Reactjs
          </details>
        </details>
        <a href="https://farmly-7e69d.firebaseapp.com/" class="visit-btn" target="blank">View app</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Works',
  methods: {
    toggleWorks() {
      const sites = document.querySelector('.sites');
      sites.classList.toggle('sites-toggle');
    }
  }
}
</script>

<style scoped>
.works {
  background-color: #64766a;
  color: #ffffff;
  width: 100%;
  padding: 1rem 0rem;
}

.works-btn {
  width: 75px;
  height: 75px;
  border-radius: 50%;
  border: 2px solid #ffffff;
  background-color: #64766a;
  color: #ffffff;
  cursor: pointer;
  text-transform: uppercase;
  font-weight: bold;
}

.works-btn:hover {
  background-color: #ffffff;
  color: #64766a;
}

.works-btn:focus {
  outline: none;
}

.sites {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  margin: 1rem 0rem;
  height: 0px;
  overflow: hidden;
  transition: 2s height;
}

.sites-toggle {
  height: 200px;
  transition: 2s height;
  overflow-y: auto;
}

.site {
  border-right: 1px solid #ffffff;
  padding: 1rem;
  width: 20%;
  min-width: 250px;
  overflow-y: auto;
}

.site:last-child {
  border-right: transparent;
}

details {
  margin-bottom: 1rem;
}

details summary {
  cursor: pointer;
}

details summary:focus {
  outline: none;
}

.visit-btn {
  text-decoration: none;
  color: inherit;
  border: 1px solid;
  border-radius: 5px;
  padding: 0.5rem 1rem;
  text-transform: uppercase;
  font-size: 0.8rem;
}

.visit-btn:hover {
  background-color: #ffffff;
  color: #64766a;
}

.hide {
  display: none;
}
</style>