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
<button
        on:click={projects}
        on:mouseenter={onHoverProjects}
        on:mouseleave={onLeave}
        class = "absolute top-1/2 left-1/2 transform -translate-x-1/5 -translate-y-1/2 w-50 h-10 opacity-0"
        >
        projects
    </button>
<button
        on:click={projects}
        on:mouseenter={onHoverAbout}
        on:mouseleave={onLeave}
        class = "absolute top-3/5 left-1/2 transform -translate-x-1/5 -translate-y-3/5 w-50 h-10 opacity-0"
        >
        About
    </button>
<button
        on:click={projects}
        on:mouseenter={onHoverLinks}
        on:mouseleave={onLeave}
        class = "absolute top-7/10 left-1/2 transform -translate-x-1/5 -translate-y-4/5 w-50 h-10 opacity-0"
        >
        Links
    </button>
</main>
