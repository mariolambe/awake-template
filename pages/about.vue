<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Mario Lambertucci"
      subtitle="SEO Expert"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
         <p>
          
          Hi, my name is Mario Lambertucci!<br>
          I have 6+ years’ experience in SEO and currently I am <b>Senior SEO Manager</b> at Zalando SE in Germany<br>
          I’ve worked on the organic expansion and the definition of SEO requirements of 18+ domains at Zalando.<br>
          Strong focus on strategies to increase rankings, from technical SEO to link acquisition and content strategies in line with company’s goals.
          </p>
          <h3>Contact me</h3>
         <p>
          
         If you need SEO support for your company or your online project feel free to reach out to me:<br>
         <b>mariolambertucci@gmail.com</b>
          </p>
        </div>
      </template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
