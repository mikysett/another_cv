<template>
  <div class="main-container">
    <MainHeader page-name="Programming" />

    <blockquote>
      “What I hear, I forget; What I see, I remember; What I do, I understand.”
      <br>
      <strong>― Confucius, 551-479 BC</strong>
    </blockquote>

    <Separator />

    <code class="prog-description">$ cat **/* | head -n 10 &amp;&amp; echo "10$?% open to speak more about it"<br>
        # C (nice), Rust (I love it), C++ (... nothing to declare)<br>
        # A bit of: Lisp, JS, Python, PHP, Go,(HTML/CSS... does it count?)<br>
        # Emacs keybindings (swapping caps lock and ctrl)<br>
        # Let's make an interactive rebase to squash those atomic commits<br>
        # Test Driven Development (and save years of my life)<br>
        # You have Windows?! Ok, I send you a Dockerfile ;)<br>
        # I've made a swagger for the API, check the entrypoints<br>
        # I have to do it more than twice? Here is a bash script<br>
        # O(1) is my goal, O(n) will be fine (please not O(n!) again!)<br>
        # Like agile, sprints, atomic tasks? me too :)<br>
        100% open to speak more about it<br>
        $ </code>

    <div class="github-stats-container">
      <h2 class="role-title">Some stats from my Github Account</h2>
      <div class="stats-img-container">
        <img src="https://github-readme-stats.vercel.app/api?username=mikysett&count_private=true&hide_rank=true" alt="Mikysett Github stats">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mikysett&layout=compact&langs_count=8&hide=hack,php,assembly,scilab" alt="">
      </div>
    </div>

    <Separator />

    <div class="extra-info-wrapper">
      <h2 class="role-title ei-title">What I loved so far</h2>
      <div class="ei-container no-p">
        <ul role="list" class="list">
          <li class="list-item">- <a href="https://en.wikipedia.org/wiki/Hackers_%26_Painters" target="_blank"
              class="text-link">Hackers &amp; Painters</a> (started my interest for functional programming)</li>
          <li class="list-item">- <a href="https://mitpress.mit.edu/9780262539807/the-elements-of-computing-systems/"
              target="_blank" class="text-link">The Elements of Computing Systems</a> (mind blowing)</li>
          <li class="list-item">- <a href="https://www.oreilly.com/library/view/exercises-in-programming/9781482227376/"
              target="_blank" class="text-link">Exercises in programming style</a> (very fun to do)</li>
          <li class="list-item">- Doing my own Bash (Aka <a href="https://github.com/mikysett/minishell" target="_blank"
              class="text-link">minishell</a><a href="https://ricette.giallozafferano.it/Parmigiana-di-melanzane.html"
              target="_blank" class="text-link"></a>)</li>
          <li class="list-item">- Starting to contribute to <a href="https://github.com/rust-lang/rust" target="_blank"
              class="text-link">rustc</a> repo (no, I didn't make any RFC, I'm not a genius)</li>
        </ul>
      </div>
    </div>

  </div>
</template>

<script>
import Separator from '@/components/Separator.vue'
import MainHeader from '@/components/MainHeader.vue'

export default {
  name: 'ProgrammingView',
  components: {
    Separator,
    MainHeader
  }
}
</script>

<style scoped>
code {
  overflow: auto;
  padding: 12px 8px;
  display: block;
  flex: 1;
  background: #300a24;
  color: #fff4ea;
  font-family: "Cutive Mono", monospace;
  font-size: 14px;
  line-height: 22px;
  white-space: nowrap;
}

.github-stats-container {
  margin-top: 20px;
}

.stats-img-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}

@media (max-width: 850px) {
  .stats-img-container {
    flex-direction: column;
  }
}
</style>
