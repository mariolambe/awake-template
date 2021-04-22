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

          Hi, my name is Mario Lambertucci!

I have 6+ years’ experience in SEO and currently I am <b>Senior SEO Manager</b> at Zalando SE in Germany 🇩🇪

I’ve worked on the organic expansion and the definition of SEO requirements of 18+ domains at Zalando.

Strong focus on strategies to increase rankings, from technical SEO to link acquisition and content strategies in line with company’s goals.


          </p>

          <h3>SEO Growth Results</h3>
          <p>
            
<b>#Project 1</b>
![SEO Growth 2](https://user-images.githubusercontent.com/61537859/114555750-4c907700-9c68-11eb-8c4a-fac26b929bc5.png)


<b>#Project 2</b>
![SEO Growth](https://user-images.githubusercontent.com/61537859/114555394-f0c5ee00-9c67-11eb-8484-a3c412a1cca8.png)
<br>
<br>

If you need SEO support for your company or your online project feel free to reach out to me:
<b>mariolambertucci@gmail.com</b>
          </p>
        </div>
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
