<template>
  <div class="lg:pt-2 pt-16 bg-[#056951]" id="packages"></div>
  <div class="BG w-full bg-[url('../assets/bg/BG2.png')] bg-no-repeat bg-cover cursor-default" >
    <div class="w-full justify-center lg:pt-20">
      <div class="w-full flex mx-auto justify-center">
        <h1 class="my-10 lg:text-7xl text-5xl text-[#4AA3AA] px-3 font-black uppercase text-outline">Packages</h1>
      </div>
      <div class="w-full flex flex-wrap mx-auto justify-center items-stretch">

        <div class="lg:w-1/4 lg:h-80 p-7 bg-[#DBDBDB] m-4 rounded-3xl self-center text-center dropshadow animate-zoom">
          <p class="text-3xl mb-2 font-bold">Online Sessions</p>
          <p class="text-base">With this package, clients will be able to experience the code camp without having to go to the workspace.</p>
          <hr class="border-solid border-4 rounded my-2">
          <ul>
          <li class="text-base">175.00 per session</li>
          <li class="text-base">2 hour sessions per weekend</li>
          <li class="text-base">8:00PM - 10:00PM</li>
          </ul>        
        </div>

        <div class="lg:w-1/4 lg:h-96 p-7 bg-[#C8C8C8] m-4 rounded-3xl self-center text-center dropshadow animate-zoom">
          <p class="text-3xl mb-2 font-bold">Onsite Sessions</p>
          <p class="text-lg">With this package, clients will be able to fully experience the code camp in a face-to-face setting.</p>
          <p class="text-lg"> Experience the atmosphere of a professional, and company-like setting.</p>
          <hr class="border-solid border-4 rounded my-2">
          <ul>
          <li class="text-lg">325.00 per session (150.00 for the payment of the workspace)</li>
          <li class="text-lg">4 hour sessions per weekend</li>
          <li class="text-lg">1:00PM - 5:00PM</li>
          </ul>  
        </div>

        <div class="lg:w-1/4 lg:h-80 p-7 bg-[#DBDBDB] m-4 rounded-3xl self-center text-center dropshadow animate-zoom">
          <p class="text-3xl mb-2 font-bold">Advanced Package</p>
          <p class="text-base">With this package, clients experienced in the field of IT, will be able to fully experience the code camp in a pace matching their knowledge. As well as dictate the setting for their learning.</p>
          <hr class="border-solid border-4 rounded my-2">
          <ul>
          <li class="text-base">175 for online or 325.00 for onsite</li>
          <li class="text-base">2 hours for online or 4 hours for onsite</li>
          <li class="text-base">8:00PM - 10:00PM for online or 1:00PM - 5:00PM for onsite</li>
          </ul>  
        </div>
        
      </div>
    </div>
  </div>
</template>

<style scoped>
.dropshadow {
  box-shadow: 8px 8px 3px 0 rgba(0, 0, 0, 0.25);
}
.text-outline {
  text-shadow: 0 0 5px white, 0 0 4px white, 0 0 4px white, 0 0 2px white;
}
.BG{
  padding-top: 1%;
  padding-bottom: 5%;
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
  animation: zoom-in 2s forwards;
}
</style>

