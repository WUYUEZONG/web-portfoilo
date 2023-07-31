<script setup>
import ContentBoard from "./components/ContentBoard.vue";
import Header from "./components/Header.vue";
import ProjectItem from "./components/ProjectItem.vue";

// const logos = ['Walmart', 'JPMorgan', 'Visa', 'Tinder', 'Samsung', 'Verizon']
</script>

<template>
  <header>
    <ContentBoard>
      <Header></Header>
    </ContentBoard>
  </header>
  <main>
    <ContentBoard>
      <div class="banner-title title">
        Helping companies build better, scalable software.
      </div>
    </ContentBoard>
    <ContentBoard>
      <div class="banner-content">
        Award-winning web developer and author, with over 15+ years of working experience with Fortune 500 companies
        like
        Apple, Google, Facebook, and more.
      </div>
    </ContentBoard>
    <ContentBoard>
      <div class="logos">
        <img src="@/assets/Logos/Walmart.svg" alt="" />
        <img src="@/assets/Logos/JPMorgan.svg" alt="" />
        <img src="@/assets/Logos/Visa.svg" alt="" />
        <img src="@/assets/Logos/Tinder.svg" alt="" />
        <img src="@/assets/Logos/Samsung.svg" alt="" />
        <img src="@/assets/Logos/Verizon.svg" alt="" />
      </div>
    </ContentBoard>
    <ContentBoard>
      <div class="projects">
        <ProjectItem></ProjectItem>
        <ProjectItem></ProjectItem>
      </div>
    </ContentBoard>
    <ContentBoard class="space-area">
      <div class="a-article">
        <span class="title">
          A co-founder at one of the world's largest communities.
        </span>
        <p>
          The combined experience I have working at the top Fortune 500 companies has allowed me to developer a skillset
          that helps me in not just development, but in every aspect of any business.
        </p>
        <p>
          I'm proud to announce that I am now working at one of the world's largest communities teaching young minds about
          how to sell yourself as a developer and open them to a whole new world of opportunities.
        </p>
        <p>
          As a developer, you have everything available to you and all that's holding you back is yourself.
        </p>
        <p>
          A quote I live by perfectly illustrates what I mean.
        </p>
        <p>
          "How big would you dream, if you knew you wouldn't fail?"
          You've already gone through the hardest parts being a developer, it's time to elevate your skills and become a
          leader in something you're passionate about.
        </p>
        <p>
          I'm happy to chat over coffee some time about how I can help your company.
        </p>
      </div>
    </ContentBoard>
    <ContentBoard>
      <div class="contact">
        <div class="title">Interested in working with me?</div>
        <div class="detail">
          I'm active on all social media platforms listed below, but you can also me an email and I will get back to you within 24-48 hours.
        </div>
        <div>
          <button>Get in touch</button>
        </div>
      </div>
    </ContentBoard>
  </main>

  <footer>
    <ContentBoard class="footer-board">
      <div class="footer">
        <span class="title">Johnathan Specter</span>
        <span class="right">
          <span>
            <img src="/src/assets/Social Icons/Twitter.svg" alt="" />
          </span>
          <span>
            <img src="/src/assets/Social Icons/LinkedIn.svg" alt="" />
          </span>
          <span>
            <img src="/src/assets/Social Icons/Github.svg" alt="" />
          </span>
        </span>
      </div>
    </ContentBoard>
  </footer>
</template>

<style>

@font-face {
  font-family: 'Inter';
  src: url('@/assets/Inter-VariableFont_slnt,wght.ttf') format('truetype');
}
@font-face {
  font-family: 'Prata';
  src: url('@/assets/Prata-Regular.ttf') format('truetype');
}

body {
  background-color: black;
  color: #c2c2c2;
  font-family: 'Inter';
  margin: 0;
  padding: 0;
}

button {
    border: 0;
    background-color: #fbe850;
    padding: 15px 30px;
    font-family: 'Prata';
}

.title {
  font-family: 'Prata';
  color: white;
}

.banner-title {
  font-size: 3.6rem;
  margin-top: 5rem;
}

.banner-title {
  max-width: 700px;
}

.banner-content {
  max-width: 620px;
}

.banner-content {
  margin: 20px 0;
  letter-spacing: 0.3px;
  line-height: 1.5rem;
}

.logos {
  display: flex;
  justify-content: space-between;
  margin: 4rem 0;
}

.projects {
  display: flex;
  justify-content: space-between;
  gap: 80px;
  flex-wrap: wrap;
}

.space-area {
  background-color: #2e3038;
  padding: 60px 0;
  margin: 60px 0;
}

.a-article {
  column-count: 2;
  column-gap: 80px;
  line-height: 1.6rem;
}
.a-article .title {
  font-size: 2.2rem;
  line-height: normal;
}

.contact {
  max-width: 520px;
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-bottom: 80px;
}
.contact .title {
  font-size: 2.2rem;
}
.contact .detail {
  font-size: 1.1rem;
  line-height: 1.6rem;
}
.footer-board {
  background-color: #2e3038;
}
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
}

.footer .right {
  display: flex;
  gap: 15px;
  padding-top: 5px;
}

@media (max-width: 767px) {
  .logos {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    row-gap: 20px;
    justify-items: center;
  }

  .logos>img:nth-child(1) {
    justify-self: right;
  }

  .banner-title {
    font-size: 3rem;
  }
  
  .a-article {
    column-count: 1;
  }
}

@media (max-width: 420px) {
  .logos {
    display: grid;
    grid-template-columns: 1fr 1fr;
    row-gap: 20px;
    justify-items: center;
  }

  .banner-title {
    font-size: 2rem;
  }

  .banner-content {
    font-size: 1rem;
  }
}</style>
