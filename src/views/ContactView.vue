<template>
    
    <section class="contact-page">
        <div class="contact-info">
            <h1 class="contact-title">Contact Me</h1>
            <p class="contact-description">
                Feel free to get in touch with me for any inquiries, collabs or just a friendy chat. You can reach out to me on the following links
            </p>
            <form @submit.prevent="submitForm" class="contact-form">
        <div class="form-group">
          <label for="name">Name:</label>
          <input type="text" id="name" v-model="formData.name" required>
        </div><br>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="formData.email" required>
        </div><br>
        <div class="form-group">
          <label for="message">Message:</label>
          <textarea id="message" v-model="formData.message" required></textarea>
        </div><br>
        <button type="submit">Submit</button>
      </form>
            <p class="contact-description">
                Email: <a href="mailto:ayanrockz@gmail.com">ayanrockz@gmail.com</a>
            </p>
            <div class="social-icons">
                <a href="https://twitter.com/?lang=en" class="social-icon">
                    <img src="twitter.webp" alt="Twitter Icon" Height="100" width="100">
                </a>
                <a href="https://au.linkedin.com" class="social-icon">
                    <img src="linkedin.png" alt="Linkedin Icon" Height="100" width="100">
                </a>
                <a href="https://github.com" class="social-icon">
                    <img src="githubss.png" alt="Github Icon" Height="100" width="100">
                </a>
            </div>
        </div>
    </section>
</template>


<script>
export default {
  data() {
    return {
      formData: {
        name: '',
        email: '',
        message: ''
      },
      formSubmitted: false
    };
  },
  methods: {
    submitForm() {
      // Implement form submission logic here
      // After successful submission, reset the form and set formSubmitted to true
      // You can also add code to send the form data to a server if needed
      
      // Example: Reset the form and set formSubmitted to true
      this.formSubmitted = true;
      this.formData = {
        name: '',
        email: '',
        message: ''
      };
    }
  }
}
</script>


<style scoped>
.contact-page {
  background-color: #f5f5f5;
  padding: 20px;
  text-align: center;
}

.contact-title {
  font-size: 28px;
  color: #333;
  margin-bottom: 20px;
}

.contact-form {
  max-width: 500px;
  margin: 0 auto;
  background-color: #fff;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

.form-group {
  margin-bottom: 20px;
}

label {
  font-size: 18px;
  color: #333;
  display: block;
  margin-bottom: 5px;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  border-radius: 3px;
}

button {
  background-color: #007BFF;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

</style>