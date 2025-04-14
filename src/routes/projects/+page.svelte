<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/formulaire");
    }
    function previous() {
        goto("/about");
    }
</script>

<header class="flex justify-center align-items-start text-[3rem] fade">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold">
        <u>Mes Projets </u>
    </h1>
</header>
<section class="flex flex-col fade">
    <div class="flex justify-center items-center flex-row">
        <a href="https://github.com/GuiguiSlide" target="_blank">
            <img
                class="rounded-full w-[10rem] h-[10rem] ml-5 mt-5 mb-10 hover:bg-[rgba(255,0,0,0.5)]"
                alt="github"
                src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/github/github-original.svg"
            />
        </a>
    </div>
    <div
        class="flex justify-center items-center text-center text-[2rem] font-bold"
    >
        <div class="flex flex-row p-5">
            <ul class="pr-20 a bg-[rgba(53,53,161,0.5)] rounded-l-4xl pl-15">
                Projets en Cours
                <a
                    href="https://www.curseforge.com/minecraft/modpacks/project-arena"
                    target="_blank"
                    ><li class="font-normal text-start hover:underline">
                        Modpack Minecraft sur le thème arène
                    </li></a
                >
                <li class="font-normal text-start">
                    Application mobile pour des recettes et des stocks
                </li>
            </ul>
            <ul class=" a bg-[rgba(130,62,194,0.5)] rounded-r-4xl pr-15 pl-45">
                Projets Finits
                <a
                    href="https://github.com/GuiguiSlide/station_m-t-o"
                    target="_blank"
                    ><li class="font-normal text-start hover:underline">
                        Station météo
                    </li></a
                >
                <a
                    href="https://github.com/GuiguiSlide/Untrustpilot/"
                    target="_blank"
                    ><li class="font-normal text-start hover:underline">
                        Site de sensibilisation sur la cybersécurité
                    </li></a
                >
                <a
                    href="https://github.com/GuiguiSlide/cassebrique"
                    target="_blank"
                    ><li class="font-normal text-start hover:underline">
                        Casse-brique en C
                    </li></a
                >
                <a
                    href="https://github.com/GuiguiSlide/projet_gamejam_2025_cesi"
                    target="_blank"
                >
                    <li class="font-normal text-start hover:underline">
                        Tower Defence GameJam 2025 au Cesi
                    </li></a
                >
            </ul>
        </div>
    </div>
</section>
<footer class="flex justify-center align-items-end fade">
    <div
        class="flex flex-row text-center justify-center space-x-100 p-10 text-[2.5rem]"
    >
        <button
            onclick={previous}
            class="bg-red-900 rounded-4xl p-5 mt-30 min-w-70 font-extrabold hover:bg-red-700"
        >
            ← précédent
        </button>
        <button
            onclick={next}
            class="bg-green-900 rounded-4xl p-5 mt-30 min-w-70 font-extrabold hover:bg-green-700"
        >
            suivant→
        </button>
    </div>
</footer>

<style>
    ul.a {
        list-style-type: circle;
    }
    .fade {
        animation-duration: 3s;
        animation-name: slide-in;
    }
    @keyframes slide-in {
        from {
            translate: 150vw 0;
            scale: 200% 1;
        }

        to {
            translate: 0 0;
            scale: 100% 1;
        }
    }

    @keyframes grow-shrink {
        25%,
        75% {
            scale: 100%;
        }

        50% {
            scale: 200%;
            color: magenta;
        }
    }
</style>
