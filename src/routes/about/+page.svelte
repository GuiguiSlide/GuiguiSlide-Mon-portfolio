<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/projects");
    }
    function previous() {
        goto("/");
    }
</script>

<header class="flex justify-center align-items-start text-[300%] fade">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold">
        <u>Mes Compétences </u>
    </h1>
</header>
<section class="flex flex-col fade">
    <div
        class="flex justify-center items-center flex-row bg-orange-200 rounded-t-4xl mr-5 ml-5 max-w-[100%] flex-wrap"
    >
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="html"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original-wordmark.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="Css"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original-wordmark.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="JS"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="C"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/c/c-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="Svelte"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/svelte/svelte-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="android"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/android/android-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="Godot"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/godot/godot-original-wordmark.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="tailwind"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original-wordmark.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="SQL"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/azuresqldatabase/azuresqldatabase-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="linux"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/linux/linux-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="flutter"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/flutter/flutter-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="powershell windows"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/powershell/powershell-original.svg"
        />
        <img
            class="rounded-4xl 3w-[2.5rem] h-[2.5rem] m-5 mt-5 mb-10"
            alt="PHP"
            src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/php/php-original.svg"
        />
    </div>
    <div
        class="flex justify-center items-center text-center text-[200%] font-bold bg-[rgba(220,120,255,0.5)] rounded-b-4xl mr-5 ml-5"
    >
        <p>
            <u>Sur cette page</u>, vous pourrez découvrir mes compétences<br />
        </p>
    </div>
</section>
<footer class="flex justify-center align-items-end fade">
    <div class="flex flex-row text-center justify-center p-10 text-[2.5rem]">
        <button
            onclick={previous}
            class="bg-red-900 rounded-4xl mr-5 p-5 mt-30 min-w-[15rem] font-extrabold hover:bg-red-700"
        >
            ← précédent
        </button>
        <button
            onclick={next}
            class="bg-green-900 rounded-4xl ml-5 p-5 mt-30 min-w-[15rem] font-extrabold hover:bg-green-700"
        >
            suivant→
        </button>
    </div>
</footer>

<style>
    .fade {
        animation-duration: 3s;
        animation-name: slide-in;
    }
    @keyframes slide-in {
        from {
            translate: 150vw 0;
            scale: 5rem 1;
        }

        to {
            translate: 0 0;
            scale: 5rem 1;
        }
    }

    @keyframes grow-shrink {
        25%,
        75% {
            scale: 5rem;
        }

        50% {
            scale: 5rem;
            color: magenta;
        }
    }
</style>
