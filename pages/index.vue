<template>
  <div>
    <div class="main-page-container">
      <div class="w-fit mx-auto">
        <div class="avatar-container">
          <img src="@/assets/images/me.jpg" class="avatar"/>
        </div>

        <div class="main-header">Egor Dushin, 19 y.o.</div>
        <!--        <div class="aka-header"><@sharapagorg></div>-->

        <div class="divider my-8"></div>

        <div class="description">
          Hey there! 👋 I'm Egor, a <span class="accent">frontend</span> developer and <span
          class="accent">freelancer</span> with four years of experience in commercial
          programming. Currently studying at <span class="accent">Innopolis University</span>, I'm embracing the student
          life while continuing to
          hone my craft. When I'm not coding, you'll likely find me hitting the <span class="accent">gym</span> or
          jamming out in the rehearsal room
          on my <span class="accent">drums</span>. Welcome to my corner of the web!
        </div>

        <div class="divider my-8"></div>

        <img
          src="@/assets/images/arrow.svg"
          class="arrow"
          @click="scrollToSecondPage"
        />
      </div>
    </div>

    <div class="w-screen min-h-screen" ref="secondPage">
      <div class="contacts-container">
        <div class="main-header">Contacts</div>

        <div class="contacts">
          <img src="@/assets/images/telegram.svg" class="contact-icon"/>
          <img src="@/assets/images/discord.svg" class="contact-icon"/>
          <img src="@/assets/images/github.svg" class="contact-icon"/>
        </div>
      </div>

      <div class="techonologies-container">

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  mounted() {

  },
  methods: {
    scrollToSecondPage() {
      this.$refs.secondPage.scrollIntoView({
        behavior: 'smooth'
      })
    }
  }
}
</script>

