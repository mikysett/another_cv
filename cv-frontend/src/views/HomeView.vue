<template>
  <div class="main-container">
    <blockquote>
      “Programs must be written for people to read, and only incidentally for machines to&nbsp;execute.”
      <br>
      <strong>― Abelson & Sussman</strong>
    </blockquote>

    <Separator />

    <div class="job-container">
      <div class="company-container">
        <div class="justified-header">
          <div class="jh-left">
            <h2 class="company-title">01Talent</h2>
          </div>
          <div class="jh-right">
            <p>Lisbon, Portugal</p>
          </div>
        </div>
        <div class="description">
          01Talent provide peer2peer learning platforms and pedagogical content to train high-level programmers worldwide.
        </div>
      </div>

      <div class="roles-wrapper">
        <div class="role-wrapper">
          <h3 class="role-title sub-role-title">Junior Software Engineer</h3>
          <div class="justified-header">
            <div class="jh-left">
              <p>Full-time</p>
            </div>
            <div class="jh-right">
              <p>Jan 2023 - Present</p>
            </div>
          </div>
          <div class="description">
            Improve the pedagogical team infrastructure creating standardized workflows and automations to streamline
            content creation and minimize friction points in production cycles.
          </div>
        </div>
        <div class="role-wrapper">
          <h3 class="role-title sub-role-title">Software Engineer Internship</h3>
          <div class="justified-header">
            <div class="jh-left">
              <p>Part-time</p>
            </div>
            <div class="jh-right">
              <p>Jul 2022 - Jan 2023</p>
            </div>
          </div>
          <div class="description">
            Implement and improve pedagogical content by creating, testing and reviewing programming exercises to provide
            reliable testers and clear content to students.
          </div>
        </div>
      </div>

      <separator />

      <div class="role-wrapper">
        <h3 class="role-title">Freelance Marketing Consultant</h3>
        <div class="justified-header">
          <div class="jh-left">
            <p>Full-time</p>
          </div>
          <div class="jh-right">
            <p>Mar 2020 - Jan 2023</p>
          </div>
        </div>
        <div class="description">
          Creating SEA marketing campaigns with particular focus in tags implementation including custom js code
          injections in order to track complex marketing funnels. Also creating simple landing pages and optimize website
          speed.
        </div>
      </div>

      <separator />

      <div class="role-wrapper">
        <h3 class="role-title">Product Subject Matter Expert</h3>
        <div class="justified-header">
          <div class="jh-left">
            <p>Teleperformance, Full-time</p>
          </div>
          <div class="jh-right">
            <p>Feb 2019 - Mar 2020</p>
          </div>
        </div>
        <div class="description">
          Focus on helping agents with complex cases and very specific scenarios empowering both colleagues and end-users
          to have the best results they can on Google Ads marketing platform.
        </div>
      </div>

    </div>

    <div class="extra-info-wrapper">
      <h2 class="role-title ei-title">Education</h2>
      <div class="ei-container">
        <h3 class="role-title">42 Lisbon School</h3>
        <div class="justified-header">
          <div class="jh-left">
            <p>Programming school</p>
          </div>
          <div class="jh-right">
            <p>2020 - 2023</p>
          </div>
        </div>
        <div class="description">Peer2peer learning with strict admission exams and real-life problems to solve in
          order to become an autonomous and versatile programmer.</div>
      </div>
      <div class="ei-container no-p">
        <h3 class="role-title">Università di Napoli L'Orientale</h3>
        <div class="justified-header">
          <div class="jh-left">
            <p>Bachelor's degree in Oriental Languages</p>
          </div>
          <div class="jh-right">
            <p>2010 - 2015</p>
          </div>
        </div>
        <div class="description">Particular focus on linguistics and socio-linguistics with a final work on the
          influence of Turkish in Arabic dialects.</div>
      </div>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import Separator from '@/components/Separator.vue'

export default {
  name: 'HomeView',
  components: {
    Separator
  }
}
</script>

<style scoped>
.company-title {
  font-size: 22px;
  line-height: 26px;
  border-left: 2px solid var(--color2);
  padding-left: 10px;
}

.roles-wrapper {
  border-left: 2px solid var(--bg3);
  padding-left: 10px;
}

.role-wrapper {
  margin: 12px 0;
}

.role-title {
  font-size: 24px;
  line-height: 30px;
  font-family: "Cutive Mono", monospace;
  margin: 0 0 10px;
}

.sub-role-title::before {
  content: "— ";
  color: var(--color2);
  font-weight: bold;
  margin-left: -10px;
}

.description {
  padding-top: 10px;
}

.extra-info-wrapper {
  margin-top: 20px;
  border: 2px solid var(--color2);
  border-radius: 4px;
  padding: 12px;
}

.ei-container {
  padding-bottom: 20px;
}

.no-p {
  padding: 0;
}

.ei-title {
  color: var(--color2);
}

</style>
