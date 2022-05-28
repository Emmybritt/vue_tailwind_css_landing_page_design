<template>
  <div class="divide-y py-3 md:px-[6rem] px-4">
      <div class="flex flex-wrap justify-center md:space-y-0 space-y-4 items-center md:justify-between py-[1rem]">
            <!--Brand Logo starts here -->
            <div>
                <h1 class="text-xl font-bold font-signika text-orange-400">Ape<span class="text-orange-600">x</span></h1>
            </div>
            <!--Brand Logo ends here-->
            <!--router link starts here-->
            <div class="flex font-bold space-x-12 capitalize ">
                <div>
                    <a href="">About</a>
                </div>
                <div>
                    <a href="">Features</a>
                </div>
                <div>
                    <a href="">Works</a>
                </div>
                <div>
                    <a href="">Supports</a>
                </div>
               
            </div>
            <!--router link ends here-->
            <div>
                <div class="md:flex hidden text-orange-500 font-bold text-sm space-x-4 items-center">
                   <a href="#" class="lab la-twitter"></a>
                   <a href="#" class="lab la-facebook-f"></a>
                   <a href="#" class="lab la-instagram"></a>
                   <a href="#" class="lab la-github"></a>
                </div>
            </div>
        </div>
        <div class="flex flex-wrap md:space-y-0 space-y-4 justify-between text-sm text-gray-500 py-3">
            <div>
                @ copywright {{ new Date().getFullYear() }} all right reserved
            </div>
            <div class="flex items-center space-x-6">
                <div>
                   <a href="">Privacy and policy</a> 
                </div>
                <div>
                   <a href="">Terms and condition</a> 
                </div>
            </div>
        </div>
  </div>
</template>

<script setup>

</script>

<style>

</style>