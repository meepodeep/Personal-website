<script lang="ts">
    import { goto } from "$app/navigation";
    function close(){
        goto ("/")
    }
</script>
<main class="w-screen h-screen object-cover overflow-hidden text-center font-osx">
    <img src= "/images/main.webp" alt="Background" class="w-full h-full object-cover absolute"/>
    <div class="text-gray-100 absolute rounded-4xl bg-gray-600 w-120 md:w-150 lg:w-200 h-150 top-[50%] left-[50%] -translate-x-1/2 -translate-y-1/2">
        <button
        on:click={close}
        class="text-center bg-gray-800 border-2 border-black rounded-md h-10 w-10 absolute top-[5%] left-[5%] -translate-x-1/2 -translate-y-1/2"
        >
            X
        </button>
        <h1 class="text-4xl my-10 "> Links! </h1>
        <div class="text-center text-blue-400 w-100 overflow-y-scroll content grid grid-cols-1 p-4 h-80 space-y-4 text-2xl sm:text-2xl md:text-3xl lg:text-4xl mx-20 md:mx-10 lg:mx-30 overscroll-contain absolute top-[50%] left-[35%] md:left-[44%] lg:left-[35%] -translate-x-1/2 -translate-y-1/2">
           <a href="https://github.com/meepodeep">GitHub</a>
           <a href="https://www.youtube.com/@meepodeepFPV/videos">YouTube</a>
           <a href="https://www.nintendo.com/us/store/products/the-legend-of-zelda-tears-of-the-kingdom-nintendo-switch-2-edition-switch-2/">Link!</a>
           <a href="https://www.printables.com/@meepodeep">Josef site!(printables)</a>
        </div>
    </div>

</main>