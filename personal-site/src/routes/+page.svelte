    <style lang="postcss">  
        @reference "tailwindcss";  
    
        :global(html) {    
            background-color: theme(--color-gray-100);  
        }
    </style>
<script lang="ts">
    let isHovered = false;
    let selected = 0;
    let img = "/images/main.png"
    import { goto } from "$app/navigation";
    import { isHttpError } from "@sveltejs/kit";

    function projects() {
        goto ('/projects');
    }
    
    function onLeave()
    {
        img = "/images/main.png"
    }
    function onHoverProjects(){
        img = "/images/projects.png"
    }
    function onHoverAbout(){
        img = "/images/About.png"
    }
    function onHoverLinks(){
        img = "/images/Links.png"
    }
</script>

<main class="w-screen h-screen overflow-hidden">
    <img src= { img } alt="Example" class="w-full h-full object-cover"/>
<!--main proj button-->
<button
        on:click={projects}
        on:mouseenter={onHoverProjects}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-3/8 left-1/2 transform -translate-x-2/6 -translate-y-1/2 w-50 h-10 opacity-0"
        >
        projects
    </button>
<!--Hack button-->
<button
        on:click={projects}
        on:mouseenter={onHoverProjects}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-1/2 left-4/6 transform -translate-x-2/6 -translate-y-3/5 w-40 h-45 opacity-0"
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
        class = "bg-amber-50 absolute top-4/9 left-1/4 transform -translate-x-1/2 -translate-y-1/4 w-80 h-75 opacity-0"
        >
        About
    </button>
<!--links button-->
<button

        on:mouseenter={onHoverLinks}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-6/11 left-6/11 transform -translate-x-5/10 -translate-y-4/5 w-35 h-10 opacity-0"
        >
        Links
    </button>
<!--links object button-->
<button

        on:mouseenter={onHoverLinks}
        on:mouseleave={onLeave}
        class = "bg-amber-50 absolute top-1/2 left-0/2 transform -translate-x-1/5 -translate-y-1/2 w-55 h-75 opacity-0"
        >
        Links
    </button>
</main>
