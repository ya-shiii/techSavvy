<template>
    <div class="bg-[#056951] lg:pt-2 pt-16" id="benefits">
        <div class="BG bg-[#056951] w-full cursor-default pt-16" >
            <div class="bg-[#D9D9D9] lg:ml-10 sm:ml-5 lg:rounded-l-3xl sm:place-content-center lg:p-5 lg:mt-20 dropshadow1">
                <h1 class="text-5xl text-center text-white lg:py-8 py-14 uppercase font-black text-outline ">like what you
                    see?</h1>
                <div class="lg:flex sm:grid lg:px-5 sm:mx-2 pb-10">
                    <div class="lg:w-3/5 sm:w-full text-xl p-5 lg:text-right text-black">
                        <p>
                            These are the benefits of choosing to partake in the Tech Savvy Code Camp, a certificate of
                            completion will be given upon creating a functioning e-Resume that clients' will be able to use
                            in applying for an IT job. Being knowledgeable in full stack web development gives you an edge
                            in the industry as you are well-rounded in the areas of web-development. Exclusive merch is
                            available per season and will be different each year. Lastly, being able to attend IT
                            conventions and experience the world of being an IT practitioner and learn from the best in the
                            industry.
                        </p>
                    </div>
                    <div class="flex justify-center w-full px-7">
                        <div class="text-xl w-full mx-auto px-7 py-4 bg-[#03372A] 
                    rounded-l-lg text-white font-semibold dropshadow animate-zoom animate-float">
                            <h2 class="text-center text-6xl font-bold mb-8">Benefits</h2>
                            <ul class="text-2xl">
                                <li class="">Certificate of Completion</li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 w-3/6">
                                <li class="">e-Resume</li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 w-3/6">
                                <li class="">Full Stack Web Development</li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 w-3/6">
                                <li class="">Exclusive Tech Savvy Merch</li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 w-3/6">
                                <li class="">Attend IT Conventions</li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 w-3/6">
                                <li class="">Learn from a Software Engineer with a decade long experience in the industry.
                                </li>
                                <hr class="border-solid border-2 rounded mb-2 border-green-300 ">
                                <!-- Add more list items as needed -->
                            </ul>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>
  
<style scoped>
.dropshadow {
    box-shadow: 7px 7px 2px 0 rgba(0, 0, 0, 0.25);
}

.text-outline {
    text-shadow: 5px 5px 0 black, 5px 5px 0 black, 5px 5px 0 black, 5px 5px 0 black;
}

.dropshadow1 {
    box-shadow: 7px 7px 2px 0 rgba(0, 0, 0, 0.25);
}

.BG {
    padding-bottom: 5%;
}

@keyframes zoom-in {
    0% {
        transform: scale(0);
        opacity: 0;
    }

    100% {
        transform: scale(1);
        opacity: 1;
    }
}

@keyframes float {
    0% {
        transform: translateY(10px);
    }

    50% {
        transform: translateY(-10px);
    }

    100% {
        transform: translateY(15px);
    }
}

.animate-zoom {
    animation: zoom-in 2s forwards;
}

.animate-float {
    animation: float 3s infinite;
}</style>
  