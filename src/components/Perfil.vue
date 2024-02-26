<script lang="ts" setup>
function social(id) {
  if (id === 0) {
    window.open("https://www.linkedin.com/in/marcosviniciussilva/", "_blank");
  }
  if (id === 1) {
    window.open("https://github.com/Animarubr", "_blank");
  }
}
</script>
<template>
  <div class="perfil-container">
    <div class="tumbnail">
      <img src="../assets/perfil.jpg" alt="profile picture" />
    </div>
    <div class="description">
      <h2>Marcos Silva</h2>
      <span>Desenvolvedor Python|Javascript</span>
    </div>
    <div class="social">
      <ph-github-logo
        @click="social(1)"
        :size="24"
        weight="fill"
        class="social-icons"
      />
      <ph-linkedin-logo
        @click="social(0)"
        :size="24"
        weight="fill"
        class="social-icons"
      />
    </div>
    <button>Resume</button>
  </div>
</template>
