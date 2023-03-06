<template>
  <div class="main-container">
    <MainHeader page-name="Bio" />

    <Separator />

    <div class="long-description">
      I've started programming when I was fourteen. First I've played with HTML and CSS and then I've bought an amazing
      manual for learning C, this is how I've discovered one of the most durable and fulfilling passions of my life (so
      far).
      <br><br>
      I've seen programming as an empowering tool to make things happen, but I was scared about making it my job, thinking
      I was not good enough.
      <br><br>
      During university (oriental cultures and languages) I've made multiple websites (with an handmade back-end in PHP)
      for couple of associations I was active in. It was an amateur theater and an environmental association. By the way,
      I deeply care about nature and I love performative art.
      <br><br>
      Growing up I've ended up working a lot in Hotels, from reception clerk to hotel manager. As an hotel manager I've
      decided to create a booking managing system since we missed one and as a receptionist on the only hotel of a private
      island I've made a guest transfer system to better coordinate boats, helicopters (oh yeah, people were coming with
      an helicopter to our hotel, I even had the chance to enjoy a free ride once) and taxis pick-ups for our guests.
      <br><br>
      In both cases our staff and guests greatly enjoyed the benefices of those applications and I experienced one more
      time how useful programming could be when applied to real-life problems.
      <br><br>
      Then life continue, I like to travel, I find myself in Lisbon, working in the SEA marketing industry.
      <br><br>
      During pandemic I discover a 42 School is opening nearby. I decide to try my chances, mainly not to have any regrets
      but feeling once again I won't be good enough to pass the one month intensive admission tests.
      <br><br>
      At my greatest surprise not only am I accepted into the school but I'm also the one that passed the tests with the
      greatest score in the entire school history in Lisbon (which now includes thousands of candidates).
      <br><br>
      From there on my goal become clearer and more linear and my experiences start to fit better into a standard CV.
      <br><br>
      I'm still a bit scared I'm not good enough, but I know now I'm definitely happy to try my best 😊
    </div>

    <Separator />

    <div class="extra-info-wrapper">
      <h2 class="role-title ei-title">When I'm not coding</h2>
      <div class="ei-container no-p">
        <ul role="list" class="list">
          <li class="list-item">🧗 Outdoor climbing! (best way to spend a week-end)</li>
          <li class="list-item">📚 Reading a nice book (currently "L'innommable" from Beckett)</li>
          <li class="list-item">🍆 Cooking traditional Italian dishes (my favorite is <a href="https://ricette.giallozafferano.it/Parmigiana-di-melanzane.html" target="_blank" class="text-link">Parmigiana</a>)</li>
          <li class="list-item">🌈 Helping out in an association that delivers hot meals to families in need<br>
            (actually I feel they are helping me more than I'm helping them)</li>
          <li class="list-item">💃 Dancing and having fun with friends</li>
      </ul>
    </div>
  </div>

</div></template>

<script>
import Separator from '@/components/Separator.vue'
import MainHeader from '@/components/MainHeader.vue'

export default {
  name: 'BioView',
  components: {
    Separator,
    MainHeader
  }
}
</script>

<style scoped></style>
