<template>
  <section class="about-me-page">
    <div class="profile-image">
      <img src="IMG_5926.jpg" alt="My picture" class="hover-effect" height="200" width="150">
    </div>
    <div class="about-content">
      <h1>About Me</h1>
      <p>
        Hello! I am Ayan, I am 19 years old and currently studying Bachelor of Information Technology. I am a passionate Web Developer. Feel free to contact me if you like my work and if you want to collaborate!
      </p>
      <p>
        I graduated from Deakin university with an IT degree, Since then, I have been working in Google as a professional Software Developer.
      </p>
      <p>
        In my free time, I like to play sports such as football and basketball. I am a great enthusiast of horse riding as well.
      </p>
      <button class="download-btn" @click="downloadFile">Download my Resume</button>
      <p>
        Thank you for visiting my portfolio. If you would like to collab or chat with me, let me know.
        Feel free to <a href="mailto:contact@gmail.com">Reach out</a>
      </p>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    downloadFile() {
      const filePath = '../CV.pdf';

      const link = document.createElement('a');
      link.href = filePath;
      link.setAttribute('download', 'CV.pdf');
      link.style.display = 'none';

      document.body.appendChild(link);
      link.click();

      document.body.removeChild(link);
    },
  },
};
</script>
