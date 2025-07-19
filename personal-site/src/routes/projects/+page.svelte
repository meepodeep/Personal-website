<script lang="ts">
    let img = "/images/ProjectsBG.webp"
</script>
<style lang="postcss">  
    @reference "tailwindcss";  
    
    :global(html) {    
        background-color: theme(--color-amber-100); 
    }
</style>
<main class="overflow-hidden font-128k-mac text-black">
    <img src= { img } alt="Example" class="w-screen h-screen object-cover"/>
    <!-- main scroll box-->
    <div class=" font-osx overscroll-contain no-scrollbar h-80 md:h-85 w-100 md:w-130 overflow-y-scroll absolute top-1/2 left-4/8 transform -translate-x-29/64 -translate-y-13/19 md:-translate-y-15/19">
    <div class="content grid grid-cols-2 p-4 space-y-4">
        <!--Delivery Drone Vid-->
         <video class="w-75 h-75 overflow-hidden rounded-2xl" controls>
            <track kind="captions">
            <source src="/images/Drone Flight.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> 
        <!--Delivery Drone Text-->
        <div>    
            <h1 class="px-2 text-l md:text-3xl">
                Delivery Drone
            </h1>   
            <h2 class="px-2 text-sm md:text-xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-xs md:text-l">
                <li>2x 2200mah 3s lipos</li>
                <li>Full autonomy using ardupilot</li>
                <li>7km range</li>
                <li>no longer working :(</li>
                <li>3d printed or foam fuselage and wings</li>
            </ul>   

            <div class="px-2">
                <h2 class="text-sm md:text-xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-xs md:text-l">
                    Not yet!
                </h3>
            </div>
        </div>   
        <img src="/images/Modular cyberdeck.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div>    
            <h1 class="px-2 text-l md:text-3xl">
                ModuDeck
            </h1>   
            <h2 class="px-2 text-sm md:text-xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-xs md:text-l">
                <li>4s lion hot swappable battery. 8 hr max battery life!</li>
                <li>Support for Lattepanda mu, pi 5, and pi zero sbc modules.</li>
                <li>Module templates to design your own!</li>
                <li>Ortholinear mechanical keyboard.</li>
                <li>Ultrawide display.</li>
            </ul>   

            <div class="px-2">
                <h2 class="text-sm md:text-xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-xs md:text-l text-blue-800">
                    <a href="https://github.com/meepodeep/modudeck">Here!</a>
                </h3>
            </div>
        </div>   
        <img src="/images/Square filler.png" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div class="item-body px-6">        
            First project
        </div>   
        <img src="/images/main.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div class="item-body px-6">        
            First project
        </div>   
        <!-- Add more as needed -->
    </div>
</div>

</main>