<template>
  <section class="content">
    <p class="title">About Me</p>
    <div class="about-me">
      <div>
        <p>
           Currently in the first year of a bachalor of IT degree at Deakin university, I am passionate about 
           I am passionate about development and in particular in 
           the web field.My ambition is to become a fullstack developer and use my knowledge and skills in business.
          </p>
      </div>
      <div>
        <img src="../assets/images/my.jpg" alt="Photo" class="me" />
      </div>
      <div>
        <p>
          My course offers me the opportunity to do an internship with the aim of validating my year.
           If you are looking for an intern and potential work-study student for the following year,
           do not hesitate to contact me by email or on linkedin .
          <a
            href="wellalanet396@gmail.com"
            class="social-link"
            aria-label="link to my mail"
            >mail</a
          >
          ou sur
          <a
            href="https://www.linkedin.com/in/nadun-adithya-a15a23194"
            target="_blank"
            class="social-link"
            aria-label="link to my linkedin"
            >linkedin</a
          >.
        </p>
      </div>
    </div>
  </section>
</template>
<style scoped>
.about-me {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.about-me > * {
  flex-basis: 25%;
  flex-grow: 0;
  flex-shrink: 0;
}

.social-link {
  position: relative;
  transition: all 300ms ease;
}

.social-link::after {
  background-color: var(--teal);
  height: 6%;
  bottom: 0;
  content: "";
  left: 0;
  min-height: 2px;
  position: absolute;
  width: 100%;
  z-index: -1;
  transition: height 300ms ease;
}

.social-link:hover::after {
  height: 100%;
}

.social-link:hover {
  color: white;
}

.me {
  border-radius: 0.5rem;
  transition: all 300ms ease;
}

.me:hover {
  transform: translateY(-0.5rem);
}

@media (max-width: 768px) {
  .about-me {
    flex-direction: column;
    gap: 1rem;
  }
}
</style>
