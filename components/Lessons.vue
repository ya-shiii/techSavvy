<template>
  <div class="BG w-full bg-[url('../assets/bg/BG.png')] bg-no-repeat bg-cover cursor-default" id="lessons">
    <div class="flex flex-col text-center w-full">
      <h1 class="mt-16 mb-10 text-6xl font-bold text-white "><span class="">WHAT WE </span><span
          class="text-white px-3 font-black text-outline text-animation">TEACH</span></h1>

      <!-- boxes content -->
      <div class="lg:flex w-full items-stretch px-5">
        <div class="bg-[#D9D9D9] self-center lg:min-h-80 lg:w-1/5 sm:w-full lg:h- m-3 py-5 px-4 text-center justify-center 
          blue-shadow animate-zoom">
          <p class="text-[#076269] font-bold text-2xl mb-10">FIGMA</p>
          <p class="lg:h-72 mb-8">Collaborative web-based application to create interface designs for User Interface and User
            Experience. The web-based UX/UI design platform allows you to work in a centralized, collaborative space where
            countless tools meet to create a unique, customized workflow.</p>
        </div>
        <div class="bg-[#D9D9D9] self-center lg:min-h-80 lg:w-1/5  sm:w-full m-3 py-5 px-4 text-center justify-center 
          blue-shadow animate-zoom">
          <p class="text-[#076269] font-bold text-2xl mb-10">HTML | CSS | JAVASCRIPT</p>
          <p class="lg:h-72 mb-10">The baseline for creating a website, these three are the languages that will be used
            primarily to create the concepts of the clients' e-Resume. HTML for formatting the layout of the website, CSS
            for the design of the website, Javascript for the functionality of the website.</p>
        </div>
        <div class="bg-[#D9D9D9] self-center lg:min-h-80 lg:w-1/5 sm:w-full m-3 py-5 px-4 text-center justify-center 
          blue-shadow animate-zoom">
          <p class="text-[#076269] font-bold text-2xl mb-10">NUXT | TAILWINDCSS | TYPESCRIPT</p>
          <p class="lg:h-72 mb-12"> The advance versions of the baseline website languages. Nuxt to be used as a framework where
            we will build websites, Tailwindcss, a CSS framework to design the website, and lastly, Typescript which is a
            language built on top of Javascript created to be a better experience than base Javascript.</p>
        </div>
        <div class="bg-[#D9D9D9] self-center lg:min-h-80 lg:w-1/5 sm:w-full m-3 py-5 px-4  text-center justify-center 
          blue-shadow animate-zoom">
          <p class="text-[#076269] font-bold text-2xl mb-10">PYTHON</p>
          <p class="lg:h-72 mb-12">Python is a general-purpose, versatile, and powerful programming language. It's a great first
            language because Python code due to its conciseness and understandability.</p>
        </div>
        <div class="bg-[#D9D9D9] self-center lg:min-h-80 lg:w-1/5 sm:w-full m-3 py-5 px-4 text-center justify-center 
          blue-shadow animate-zoom">
          <p class="text-[#076269] font-bold text-2xl mb-10">DJANGO</p>
          <p class="lg:h-72 mb-6">Django is a high-level Python web framework that encourages rapid development and clean,
            pragmatic design. Django is a back-end server side web framework. Django is free, open source and written in
            Python making it easier to build web pages using Python.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.text-outline {
  -webkit-text-fill-color: black;
  -webkit-text-stroke: 3px;
}

.blue-shadow {
  box-shadow: 7px 7px 2px 0 rgba(100, 180, 186, 0.5);
}

.BG {
  padding-top: 5%;
}

@keyframes zoom-in {
  0% {
    opacity: 0;
    transform: scale(0.2);
  }

  100% {
    opacity: 1;
    transform: scale(1);
  }
}

.animate-zoom {
  animation: zoom-in 1s forwards;
}

@keyframes typing {
  0% {
    opacity: 0;
    transform: translateX(-10px);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.text-animation {
  display: inline-block;
  opacity: 0;
  animation: typing 2s ease-in-out;
  animation-fill-mode: forwards;
}

.text-animation:nth-child(2) {
  animation-delay: 0.2s;
}

.text-animation:nth-child(3) {
  animation-delay: 0.4s;
}

.text-animation:nth-child(4) {
  animation-delay: 0.6s;
}

.text-animation:nth-child(5) {
  animation-delay: 0.8s;
}

.text-animation:nth-child(6) {
  animation-delay: 1s;
}</style>