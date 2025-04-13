<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/about");
    }
    function previous() {
        goto("/");
    }
</script>

<header class="flex justify-center align-items-start text-[3rem]">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold">
        <u>Mes Compétences </u>
    </h1>
</header>
<section class="flex flex-col">
    <div class="flex justify-center items-center flex-row">
        <img
            class="rounded-4rem w-[10rem] h-[10rem] mt-5 mb-10"
            alt="html"
            src="https://soltech.net/wp-content/uploads/2014/05/HTML5.webp"
        />
        <img
            class="rounded-4rem w-[10rem] h-[10rem] pl-8 mt-5 mb-10"
            alt="Css"
            src="https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg"
        />
        <img
            class="rounded-4rem w-[15rem] h-[10rem] mt-5 mb-10"
            alt="JS"
            src="https://1000logos.net/wp-content/uploads/2020/09/JavaScript-Logo-500x313.png"
        />
        <img
            class="rounded-4rem w-[10rem] h-[10rem] mt-5 mb-10"
            alt="C"
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/C_Programming_Language.svg/1200px-C_Programming_Language.svg.png"
        />
        <img
            class="rounded-4rem w-[10rem] h-[10rem] ml-10 mt-5 mb-10"
            alt="Godot"
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Godot_icon.svg/2048px-Godot_icon.svg.png"
        />
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
        <p>
            sur cette pages vous pourrez decouvrir mes compétences<br />
        </p>
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
</style>
