<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/");
    }
    function previous() {
        goto("/about");
    }
</script>

<header class="flex justify-center align-items-start text-[3rem]">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold">
        <u>Mes Projets </u>
    </h1>
</header>
<section class="flex flex-col">
    <div class="flex justify-center items-center flex-row">
        <a href="https://github.com/GuiguiSlide" target="_blank">
            <img
                class="rounded-full w-[10rem] h-[10rem] ml-5 mt-5 mb-10"
                alt="github"
                src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABwAAAAcCAMAAABF0y+mAAAAeFBMVEUjHyAiHyAjHiAiHiAgHB0UDRAAAAAaFReEgoPBwMDf39/v7++2trb///+xsLBzcnL+/v5qaGmWlZWMiosJAAAMAAUeGRtCP0Chn6BZV1hRT1A2MjPZ2dlfXV08OTpKSEjQz89lY2MXEhR9e3z19fXHxsbn5+cqJifS2g27AAABfElEQVR4AWVRBaLkUAjjGUzdfdz2/jdcoLLyU6PQlBAAwDBgg9nuZousBef47gMqgge7Fvgra53lEtIpipMkjk4BvZO03X7kgk+zAzmFo40xDovsb5QVMscpzWHNCcHxaHDntqfsB4rOqqx+4JdxivZ8Oud8X3pVjGeOLx3OxZXoWtywqzhxR6HSxJ2yBwE9e+/7Zw9PlXcjZmIkxeqpUyueLx2oBXD4Xn8iNTnd1ijhlF+E+Aq7rzJeOHEqAw/9LIE2gN11umSMoRc9jInU6b1ppYp66G/CPAWrTutpQyPFaw++l+CD8AcG72Jw5zj6CnXmcF9iqy3PyGE3bovoVBS124pqGcD/YvN4LfHILgFV+TdTkJd1IvusXkvxuW92bLWJwySLu/GeomhF3Wn2RY6ZCXQtsxGf6MUfVN576Xe/nsM7K7+JyFuLyfUJByh8OIU7M+rIbIM5Pj1OH2YaywI+M3ony1nL1lggRH13iLTayGqMAGA95eb22JjfaOUa5/ipzPYAAAAASUVORK5CYII="
            />
        </a>
    </div>
    <div
        class="flex justify-center items-center text-center text-[2rem] font-bold"
    >
        <div class="flex flex-row p-5">
            <ul class="pr-20 a">
                Projets en Cours
                <a href="https://www.curseforge.com/minecraft/modpacks/project-arena"><li class="font-normal text-start hover:underline">
                    Modpack Minecraft sur le thème arène
                </li></a>
                <li class="font-normal text-start">
                    Application mobile pour des recettes et des stocks
                </li>
            </ul>
            <ul class="pl-20 a">
                Projets Finits
                <a href="https://github.com/GuiguiSlide/station_m-t-o"><li class="font-normal text-start hover:underline">Station météo</li></a>
                <a href="https://github.com/GuiguiSlide/Untrustpilot/"><li class="font-normal text-start hover:underline">Site de sensibilisation sur la cybersécurité</li></a>
                <a href="https://github.com/GuiguiSlide/cassebrique"><li class="font-normal text-start hover:underline" >Casse-brique en C</li></a>
                <a href="https://github.com/GuiguiSlide/projet_gamejam_2025_cesi"> <li class="font-normal text-start hover:underline">Tower Defence GameJam 2025 au Cesi</li></a>
            </ul>
        </div>
    </div>
</section>
<footer class="flex justify-center align-items-end">
    <div
        class="flex flex-row text-center justify-center space-x-100 p-10 text-[2.5rem]"
    >
        <button
            onclick={previous}
            class="bg-red-900 rounded-4xl p-5 mt-30 min-w-70 font-extrabold hover:bg-red-700"
        >
            ← previous
        </button>
        <button
            onclick={next}
            class="bg-green-900 rounded-4xl p-5 mt-30 min-w-70 font-extrabold hover:bg-green-700"
        >
            next →
        </button>
    </div>
</footer>

<style>
    ul.a {
        list-style-type: circle;
    }
</style>
