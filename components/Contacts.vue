<template>
  <div class="bg-black text-white cursor-default w-full">
    <div class="lg:pt-2 pt-16 w-full" id="contacts"></div>
    <footer class="contact-section flex flex-wrap justify-between">
      <div class="column mb-8">
        <h1 class="text-center mb-2 text-3xl font-bold">About Us</h1>
        <div class="intro text-center">
          <p class="mt-5 text-2xl font-bold">Welcome to Tech Savvy</p>
          <p class="mt-5 font-bold">Address</p>
          <p>In front of Ozamiz City Hall, 2nd floor of Mercury Drug/SSS, Ozamiz, Philippines</p>
          <p class="mt-5 font-bold">Email Address</p>
          <p>info@codecamp-techsavvy.com</p>
          <p>codedevsolutions@gmail.com</p>
        </div>
      </div>
      <div class="column mb-8">
        <h1 class="text-center mb-2 text-3xl font-bold">Contact Us</h1>
        <form action="https://formspree.io/f/xgejvwgd" method="POST">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" class="h-8" required>
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" class="h-8" required>
          <label for="message">Message:</label>
          <textarea id="message" name="message" class="h-20" required></textarea>
          <button type="submit" class="bg-teal-700 text-white px-4 py-2">Send Message</button>
        </form>
      </div>
      <div class="column mb-10">
        <h1 class="text-center mb-2 text-3xl font-bold">Follow Us</h1>
        <div class="social-icons text-black">
  <a href="https://www.facebook.com/TechSavvyCodeCamp" target="_blank" class="btn bg-teal-700 cursor-pointer">Facebook</a>
  <a href="https://www.instagram.com/tech_savvy2023" target="_blank" class="btn bg-teal-700 text-black cursor-pointer">Instagram</a>
</div>

      </div>
      <div class="w-full text-center text-white">
        <p>©2023 TechSavvy Codecamp</p>
      </div>
    </footer>
  </div>
</template>

<style>
.intro {
  font-size: larger;
}

.bg {
  background-color: #73a9ad;
}

.contact-section {
  @apply flex flex-wrap justify-between;
}

.column {
  @apply w-full sm:w-1/2 lg:w-1/3 p-4;
}

.column h1 {
  @apply mb-2 text-3xl font-bold;
}

form {
  @apply grid grid-cols-1 gap-4;
}

form label {
  @apply block;
}

form input,
form textarea,
form button {
  @apply w-full;
}

.social-icons {
  @apply space-y-4 grid grid-rows-1 justify-center mt-8;
}

.btn {
  @apply inline-block px-4 py-4 px-32 text-center rounded text-white;
}

.btn:hover {
  @apply opacity-75;
}

@media (min-width: 640px) {
  .column {
    @apply w-1/2;
  }
}

@media (min-width: 768px) {
  .column {
    @apply w-1/3;
  }
}
</style>
