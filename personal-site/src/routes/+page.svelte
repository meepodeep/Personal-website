    <style lang="postcss">  
        @reference "tailwindcss";  
    
        :global(html) {    
            background-color: theme(--color-gray-100);  
        }
    </style>
<script lang="ts">
    let isHovered = false;
    let selected = 0;
    let img = "/images/main.webp"
    import { goto } from "$app/navigation";
    import { isHttpError } from "@sveltejs/kit";

    function projects() {
        goto ('/projects');
    }
    
    function onLeave()
    {
        img = "/images/main.webp"
    }
    function onHoverProjects(){
        img = "/images/projects.webp"
    }
    function onHoverAbout(){
        img = "/images/About.webp"
    }
    function onHoverLinks(){
        img = "/images/Links.webp"
    }
</script>

<main class="w-screen h-screen overflow-hidden relative">
    <img src= { img } alt="Background" class="w-full h-full object-cover absolute"/>
<!--main proj button-->
<button
        on:click={projects}
        on:mouseenter={onHoverProjects}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-[36%] left-[52%] w-50 h-10 -translate-x-1/2 -translate-y-1/2 opacity-0"
        >
        projects
    </button>
<!--Hack button-->
<button
        on:click={projects}
        on:mouseenter={onHoverProjects}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-1/2 left-4/6 transform -translate-x-2/6 -translate-y-3/5 w-40 h-45 sm:opacity-0 hidden lg:block"
        >
        projects
    </button>
<!--About button-->
<button

        on:mouseenter={onHoverAbout}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-4/9 left-1/2 transform -translate-x-1/5 -translate-y-1/2 w-50 h-10 opacity-0"
        >
        About
    </button>
<!--Machine button-->
<button

        on:mouseenter={onHoverAbout}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-4/9 left-1/4 transform -translate-x-1/2 -translate-y-1/4 w-80 h-75 sm:opacity-0 hidden lg:block"
        >
        About
    </button>
<!--links button-->
<button

        on:mouseenter={onHoverLinks}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-[54%] left-[55%] transform -translate-x-1/2 -translate-y-1/2 w-35 h-10 opacity-0"
        >
        Links
    </button>
<!--links object button-->
<button

        on:mouseenter={onHoverLinks}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-1/2 left-0/2 transform -translate-x-1/5 -translate-y-1/2 w-55 h-75 sm:opacity-0 hidden lg:block"
        >
        Links
    </button>
</main>
