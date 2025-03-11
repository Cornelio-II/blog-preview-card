<template>
  <div class="card-container">
    <header aria-label="Blog preview card">
      <img src="/illustration-article.svg?url" alt="illustration-article" type="image/svg" />

    </header>
    <main>
      <h2>Learning</h2>
      <span>Published 21 Dec 2023</span>
      <section>
        <h1> HTML & CSS foundations</h1>
        <p> These languages are the backbone of every website, defining structure, content, and presentation.</p>
      </section>
      <aside>
        <div class="author">
          <img srcset="/image-avatar.webp" class="image-avatar" alt="avatar-michelle" type="image/webp" />
          Greg Hooper
        </div>
      </aside>
    </main>
  </div>

  <footer>
    <p> Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
      Coded by <a href="https://github.com/Timex29/blog-preview-card">Cornelio</a>.</p>
  </footer>
</template>
<style scoped>
.card-container {
  background-color: var(--white);
  border-radius: 0.625rem;
  box-shadow: 0.625rem 0.625rem 0.2rem var(--gray-950);
  margin: 0 auto;
  border: 0.063rem solid var(--gray-950);
  padding: 1rem;
  width: 18.75rem;
  overflow: hidden;
  margin: 2rem auto;
}

header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 1rem;
}

img {
  width: 100%;
  height: auto;
  border-radius: 0.625rem;
}

h1 {
  font-size: clamp(1rem, 1rem + 1vw, 1.5rem);
  margin-bottom: 0.5rem;
  font-weight: bold;
  color: var(--gray-950);
}

h1:hover {
  color: var(--yellow);
}

h2 {
  color: var(--gray-950);
  font-weight: bold;
  background-color: var(--yellow);
  border-radius: 0.375rem;
  padding: 0.25rem 0.5rem;
  align-items: left;
  width: fit-content;
  font-size: medium;
}

span {
  color: var(--gray-500);
  font-size: 0.8rem;
  font-weight: bold;
}

main {
  margin-bottom: 1rem;
}

p {
  color: var(--gray-500);
  font-size: clamp(0.7rem, 0.7rem + 0.5vw, 1rem);
  margin-bottom: 1rem;
}
aside {
  margin-top: 2rem;
}
.image-avatar {
  width: 2rem;
  height: 2rem;
  border-radius: 50%;
  overflow: hidden;
  margin-right: 0.5rem;
}

.author {
  display: flex;
  align-items: center;
  font-size: clamp(0.6rem, 0.6rem + 0.5vw, 0.9rem);
  font-weight: bold;
  color: var(--gray-950);
  zoom: 1;
}

footer {
  margin: 2rem 0;
}

@media screen and (min-width: 48rem) {
  .card-container {
    width: 22.5rem;
  }

  footer {
    text-align: center;
  }
}
</style>
