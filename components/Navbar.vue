<script setup>
import { ref } from 'vue';

const isMobileMenuOpen = ref(false);

const scrollToSection = (sectionId) => {
  const section = document.getElementById(sectionId);
  if (section) {
    section.scrollIntoView({ behavior: 'smooth' });
    toggleMobileMenu();
  }
};

const toggleMobileMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};
</script>

<template>
  <div class="navbar fixed top-0 left-0 w-full z-50 bg-[#03372A] cursor-pointer ">
    <div class="container mx-auto px-4">
      <div class="flex justify-between items-center sm:py-0 py-4">

        <!-- Mobile Menu Toggle -->
        <button @click="toggleMobileMenu" class="sm:hidden">
          <svg class="h-8 w-10" fill="white" viewBox="0 0 14 20">
            <path v-if="!isMobileMenuOpen" fill-rule="evenodd" clip-rule="evenodd" 
            d="M3 4.5C3 4.22386 3.22386 4 3.5 4H16.5C16.7761 4 17 4.22386 17 4.5C17 4.77614 
              16.7761 5 16.5 5H3.5C3.22386 5 3 4.77614 3 4.5ZM3 9.5C3 9.22386 3.22386 9 3.5 
              9H16.5C16.7761 9 17 9.22386 17 9.5C17 9.77614 16.7761 10 16.5 10H3.5C3.22386 10 
              3 9.77614 3 9.5ZM16.5 15C16.7761 15 17 14.7761 17 14.5C17 14.2239 16.7761 14 16.5 
              14H3.5C3.22386 14 3 14.2239 3 14.5C3 14.7761 3.22386 15 3.5 15H16.5Z"></path>
            <path v-else fill-rule="evenodd" clip-rule="evenodd" d="M3.00391 4.49991C3.00391 
              4.22377 3.22777 3.99991 3.50391 3.99991H16.5039C16.78 3.99991 17.0039 4.22377 17.0039 
              4.49991C17.0039 4.77606 16.78 4.99991 16.5039 4.99991H3.50391C3.22777 4.99991 3.00391 
              4.77606 3.00391 4.49991ZM3.00391 9.49991C3.00391 9.22377 3.22777 8.99991 3.50391 
              8.99991H16.5039C16.78 8.99991 17.0039 9.22377 17.0039 9.49991C17.0039 9.77606 16.78 
              9.99991 16.5039 9.99991H3.50391C3.22777 9.99991 3.00391 9.77606 3.00391 9.49991ZM3.00391 
              14.4999C3.00391 14.2238 3.22777 13.9999 3.50391 13.9999H16.5039C16.78 13.9999 17.0039 
              14.2238 17.0039 14.4999C17.0039 14.7761 16.78 14.9999 16.5039 14.9999H3.50391C3.22777 
              14.9999 3.00391 14.7761 3.00391 14.4999Z"></path>
          </svg>

        </button>

        <!-- Desktop Navbar -->
        <nav class="hidden sm:block ">
          <ul class="flex space-x-4">
            <li><a class="navbar-link" @click="scrollToSection('home')">Home</a></li>
            <li><a class="navbar-link" @click="scrollToSection('vmo')">VMO</a></li>
            <li><a class="navbar-link" @click="scrollToSection('lessons')">Lessons</a></li>
            <li><a class="navbar-link" @click="scrollToSection('benefits')">Benefits</a></li>
            <li><a class="navbar-link" @click="scrollToSection('packages')">Packages</a></li>
            <li><a class="navbar-link" @click="scrollToSection('testimonies')">Testimonies</a></li>
            <li><a class="navbar-link" @click="scrollToSection('contacts')">Contacts</a></li>
          </ul>
        </nav>
      </div>
    </div>

    <!-- Mobile Menu -->
    <div v-if="isMobileMenuOpen" class="sm:hidden bg-[#03372A] drop-shadow-md">
      <ul class="py-2 px-4">
        <li><a class="block py-2 navbar-link" @click="scrollToSection('home')">Home</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('vmo')">VMO</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('lessons')">Lessons</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('benefits')">Benefits</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('packages')">Packages</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('testimonies')">Testimonies</a></li>
        <li><a class="block py-2 navbar-link" @click="scrollToSection('contacts')">Contacts</a></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.navbar-link {
  @apply inline-block px-4 py-3 text-white uppercase font-bold;
  @apply hover:text-white;
}

.navbar-link:hover {
  @apply bg-teal-700;
}
</style>
