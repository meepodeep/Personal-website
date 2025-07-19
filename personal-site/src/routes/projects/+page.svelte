<script lang="ts">
    let img = "/images/ProjectsBG.png"
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
    <div class="bg-amber-50 font-osx overscroll-contain no-scrollbar h-1/2 w-75 md:w-4/12 overflow-y-scroll absolute top-1/2 left-4/8 transform -translate-x-29/64 -translate-y-6/8">
    <div class="content grid grid-cols-2 p-4 space-y-4">
         <video class="w-75 h-75 overflow-hidden rounded-2xl" controls>
            <track kind="captions">
            <source src="/images/Drone Flight.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> 
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
                <li>3d printed or foam frame</li>
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
        <img src="/images/Square filler.png" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div class="item-body px-6">        
            First project
        </div>   
        <img src="/images/Square filler.png" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div class="item-body px-6">        
            First project
        </div>   
        <img src="/images/main.png" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div class="item-body px-6">        
            First project
        </div>   
        <!-- Add more as needed -->
    </div>
</div>

</main>