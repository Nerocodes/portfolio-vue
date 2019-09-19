<template>
  <section class="works">
    <button class="works-btn" @click="toggleWorks">View my works</button>
    <div class="sites">
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
        <a href="https://temitopeodushola.com/" class="visit-btn" target="blank">View app</a>
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
      <div class="site">
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
        <p class="title">Teelonis</p>
        <p class="description">All about gifts</p>
        <details>
          <summary>Stack</summary>
          <details>
            <summary>Frontend</summary>
            Vuejs
          </details>
        </details>
        <a href="https://teelonis.herokuapp.com/" class="visit-btn" target="blank">View app</a>
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
  background-color: #001947;
  color: #ffffff;
  width: 100%;
}

.works-btn {
  width: 75px;
  height: 75px;
  border-radius: 50%;
  border: 2px solid #ffffff;
  background-color: #001947;
  color: #ffffff;
  cursor: pointer;
  text-transform: uppercase;
  font-weight: bold;
}

.works-btn:hover {
  background-color: #ffffff;
  color: #001947;
}

.works-btn:focus {
  outline: none;
}

.sites {
  display: flex;
  justify-content: center;
  margin: 1rem 0rem;
  height: 0px;
  overflow: hidden;
  transition: 2s height;
}

.sites-toggle {
  height: 200px;
  transition: 2s height;
}

.site {
  border-right: 1px solid #ffffff;
  padding: 1rem;
  width: 25%;
  overflow-y: auto;
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
  color: #001947;
}
</style>