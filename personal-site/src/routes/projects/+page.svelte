<script lang="ts">
    let img = "/images/ProjectsBG.webp";
    let code = "Welcome to the projects page! :)";
    let page = "/wpp page";
    import { goto } from "$app/navigation";
    function wwp() {
        goto (page)
    }
    function close(){
        goto ("/")
    }
    function onHoverWwp(){
        if (code == "projects page page"){
            page = "/wpp page"
        }else{
            page = ""
        }
        img = "/images/floppy disk.webp";
    }
    function onLeave(){
        img = "/images/ProjectsBG.webp";
    }
</script>
<style lang="postcss">  
    @reference "tailwindcss";  
    
    :global(html) {    
        background-color: theme(--color-amber-100); 
    }
</style>
<main class="overflow-hidden font-128k-mac text-black">
    <img src= { img } alt="Background" class="w-screen h-screen object-cover"/>
    <button
        on:click={close}
        class="bg-white border-2 border-black font-osx h-7 w-7 absolute top-[20%] left-[5%] md:left-[15%] lg:left-[37%] -translate-x-1/2 -translate-y-1/2"
        >
            X
    </button>
    <input bind:value={code} class = "absolute top-[20%] left-[38%] -translate-y-1/2 -translage-x-1/2 bg-white w-100 border-black border-2 font-osx hidden lg:block" placeholder="Welcome to the projects page! :)">
    <button
        on:click={wwp}
        on:mouseenter={onHoverWwp}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-[80%] left-[63%] w-70 h-10 -translate-x-1/2 -translate-y-1/2 opacity-0"
        >
        projects
    </button>
    <!-- main scroll box-->
    <div class="font-osx overscroll-contain no-scrollbar h-70 md:h-100 lg:h-75 w-85 md:w-120 lg:w-140 overflow-y-scroll absolute top-[50%] lg:top-[51%] left-4/8 transform -translate-x-32/64 md:-translate-x-29/64 lg:-translate-x-29/64 -translate-y-15/19">
    <div class="content grid grid-cols-2 p-4 space-y-4">
        <!--Delivery Drone Vid-->
         <video class="pt-4 w-75 h-75 overflow-hidden rounded-2xl" controls>
            <track kind="captions">
            <source src="/images/Drone Flight.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video> 
        <!--Delivery Drone Text-->
        <div class="pt-4">    
            <h1 class="px-2 text-l md:text-2xl lg:text-3xl">
                Delivery Drone
            </h1>   
            <h3 class="px-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                flying wing delivery drone
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>2x 2200mah 3s lipos</li>
                <li>Full autonomy using ardupilot</li>
                <li>7km range</li>
                <li>no longer working :(</li>
                <li>3d printed or foam fuselage and wings</li>
            </ul>   

            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                    Not yet!
                </h3>
            </div>
        </div>   
        <img src="/images/Modular cyberdeck.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />     
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                ModuDeck
            </h1>   
            <h3 class="px-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                Fully modular cyberdeck
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Modular batteries and compute modules!</li>
                <li>Open source modules!</li>
                <li>Ortholinear keyboard!</li>
            </ul>   

            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="https://github.com/meepodeep/modudeck">Here!</a>
                </h3>
            </div>
        </div>   
        <img src="/images/ErgoDecks.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                ErgoDecks
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                Split Ergo Keyboard
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Two Bluetooth halves</li>
                <li>Choc switch compatability</li>
                <li>2x 100mah lipos</li>
            </ul>   
            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="https://github.com/meepodeep/ergoDecks">Here!</a>
                </h3>
            </div>
        </div>
        <img src="/images/pedals.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                Pedals
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                Flight sim pedals
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Reads as a gamepad joystick</li>
                <li>Works with any game</li>
                <li>90% 3d printed</li>
            </ul>   
            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="">not yet</a>
                </h3>
            </div>
        </div>
        <img src="/images/drone.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                5in Drone 
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                5in fpv drone
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Expresslrs radio link</li>
                <li>Caddx vista vtx (not shown)</li>
                <li>Betaflight</li>
            </div>
        <img src="/images/turbine.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                Wind turbine
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                3d printed wind turbine
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Stepper generator</li>
                <li>Dual bridge rectifier in series</li>
                <li>90% 3d printed</li>
                <li>Test bench for airfoil efficiency</li>
            </ul>   
            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="">not yet</a>
                </h3>
            </div>
        </div>
        <!--ebrake -->
         <img src="/images/ebrake.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                sim handbrake
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                handbrake for racing simulators
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>Hall sensor</li>
                <li>sturdy aluminum construction</li>
                <li>laser cut side windows</li>
            </ul>   
            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="https://github.com/meepodeep/sim-ebrake">Here!</a>
                </h3>
            </div>
        </div>
        <!-- shifter -->
          <img src="/images/shifter.webp" class="rounded-lg shadow-md shrink" alt="Image 1" />    
        <div>    
            <h1 class="px-2 text-l md:text-xl lg:text-3xl">
                sim shifter
            </h1>   
            <h3 class="px-2 pt-2 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                notchy shifter for racing simulators
            </h3>
            <h2 class="pl-2 text-sm md:text-xl lg:text-2xl">
                Features
            </h2>
            <ul class="list-disc px-6 text-tiny md:text-sm lg:text-l 2xl:text-xl">
                <li>realistic feeling shifting</li>
                <li>mostly 3d printed</li>
                <li>works with any sim</li>
            </ul>   
            <div class="px-2">
                <h2 class="text-sm md:text-xl lg:text-2xl">
                    GitHub
                </h2>
                <h3 class="px-4 text-tiny md:text-sm lg:text-l 2xl:text-xl text-blue-800">
                    <a href="https://github.com/meepodeep/sim-shifter">Here!</a>
                </h3>
            </div>
        </div>
        <!--add more as needed-->
    </div>
</div>

</main>