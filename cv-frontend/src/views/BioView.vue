<template>
  <div class="main-container">
    <MainHeader page-name="Bio" />

    <Separator />

    <div class="long-description">
      I started programming when I was fourteen. First I played with HTML and
      CSS and then I bought an amazing manual for learning C. This is how I
      discovered one of the most durable and fulfilling passions of my life (so
      far).<br /><br />
      I used to see programming as an empowering tool to make things happen, but
      I was scared of making it my job, thinking I was not good enough.<br /><br />
      During university (oriental cultures and languages) I made multiple
      websites (with a handmade back-end in PHP) for a couple of associations I
      was active in, an amateur theater and an environmental association. By the
      way, I deeply care about nature and I love performative art.<br /><br />
      Growing up I ended up working a lot in hotels, from reception clerk to
      hotel manager. As a hotel manager I decided to create a
      <a
        href="https://github.com/mikysett/horrible_booking_system"
        target="_blank"
        class="text-link"
        >booking managing system</a
      >
      since we missed one and as a receptionist in the only hotel of a private
      island I made a
      <a
        href="https://github.com/mikysett/horrible_guest_transfer_system"
        target="_blank"
        class="text-link"
        >guest transfer system</a
      >
      to better coordinate boats, helicopters (oh yeah, people were coming with
      a helicopter to our hotel, I even had the chance to enjoy a free ride
      once) and taxi pick-ups for our guests.<br /><br />
      In both cases the staff and guests greatly enjoyed the benefits of those
      applications and I experienced one more time how useful programming can be
      when applied to real-life problems.<br /><br />
      Then life went on and my passion for travel brought me to Lisbon, where I
      started working in the SEA marketing industry.<br /><br />
      During the pandemic I discovered that a
      <a href="https://www.42network.org/" target="_blank" class="text-link"
        >42 School</a
      >
      was opening nearby. I decided to try my chances and started the one month
      intensive admission tests.<br /><br />
      To my greatest surprise not only was I accepted into the school but to
      date I'm also the one that passed the tests with the greatest score in the
      entire school history in Lisbon (which now includes thousands of
      candidates).<br /><br />
      From there on my goal became clearer and more linear and my experiences
      started to fit better into a standard CV.<br /><br />
      I'm still a bit scared I'm not good enough, but now I know I'm definitely
      happy to try my best 😊
    </div>

    <Separator />

    <div class="extra-info-wrapper">
      <h2 class="role-title ei-title">When I'm not coding</h2>
      <div class="ei-container no-p">
        <ul role="list" class="list">
          <li class="list-item">
            🧗 Outdoor climbing! (best way to spend a week-end)
          </li>
          <li class="list-item">
            💃 Dancing Forrò (an amazing north-brasilian dance)
          </li>
          <li class="list-item">
            📚 Reading a nice book (currently "Scritto contro Marx" from
            Bakunin)
          </li>
          <li class="list-item">
            🍆 Cooking traditional Italian dishes (my favorite is
            <a
              href="https://ricette.giallozafferano.it/Parmigiana-di-melanzane.html"
              target="_blank"
              class="text-link"
              >Parmigiana</a
            >)
          </li>
          <li class="list-item">
            🌈 Helping out in an association that delivers hot meals to families
            in need<br />
            (actually I feel they are helping me more than I'm helping them)
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

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
