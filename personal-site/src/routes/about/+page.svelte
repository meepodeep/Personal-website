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
        <h1 class="text-4xl my-10 "> About! </h1>
        <p class="text-l sm:text-l md:text-xl lg:text-xl mx-20 md:mx-10 lg:mx-30 ">
            Self described mechanical engineer who was forced to code. I'm also mildly obsessed with coffee if you couldnt tell. I have been making projects involving electronics, programming, and 3d printing for around 7 years as of now,
             and I have built many things from delivery drones to vr games. You will hopefully see me around the Hack Club slack as @meepodeep, see you there!
        </p>
    </div>

</main>