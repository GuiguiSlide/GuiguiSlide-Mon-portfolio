<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/about");
    }
    function previous() {
        goto("/");
    }
    function linkedin() {
        window.open(
            "https://www.linkedin.com/in/guillaume-beaufort-ba252932a/",
            "_blank",
        );
    }
</script>

<header class="flex justify-center align-items-start text-[150%] fade">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold pl-20 pr-20">
        <u>Bienvenue sur mon Portfolio </u>
    </h1>
</header>
<section class="flex flex-col fade">
    <div class="flex justify-center items-center">
        <!-- svelte-ignore a11y_no_static_element_interactions -->
        <!-- svelte-ignore a11y_click_events_have_key_events -->
        <div
            class="photoprofil rounded-full w-[15rem] h-[15rem] m-10"
            onclick={linkedin}
            alt="Guillaume Beaufort LinkedIn"
        >
            <br /><br /><br /><br /><br /><br /><br /><br />
        </div>
    </div>
    <div
        class="flex justify-center items-center text-center text-[150%] font-bold bg-[rgba(219,100,199,0.5)] pb-10 pt-10 rounded-4xl ml-20 mr-20"
    >
        <p>
            Bienvenue sur mon profile,<br /> je suis Guillaume Beaufort un Developpeur
            FullStack en formation au CESI de brest.,
        </p>
    </div>
</section>
<footer class="flex justify-center align-items-end fade">
    <div
        class="flex flex-row text-center justify-center space-x-100 p-10 text-[150%]"
    >
        <button
            onclick={next}
            class="bg-green-900 rounded-4xl p-5 mt-30 min-w-[150%] font-extrabold hover:bg-green-700"
        >
            suivant→
        </button>
    </div>
</footer>

<style>
    .photoprofil {
        background: url("https://media.licdn.com/dms/image/v2/D4D03AQF_N2UKIIZUrg/profile-displayphoto-shrink_800_800/B4DZPZIdIkHgAg-/0/1734514693126?e=1750291200&v=beta&t=uy0reay1cNdXeYPJtiRNYxV6z6nySdHMR4pkaZz74Zk");
        background-size: cover;
        background-position: center;
    }
    .photoprofil:hover {
        background: url("https://media.licdn.com/dms/image/v2/C560BAQHaVYd13rRz3A/company-logo_100_100/company-logo_100_100/0/1638831590218/linkedin_logo?e=1749686400&v=beta&t=yLR0Vlcq_i5T8596-RjRSVQMOOCNb9b9X7OshdnJjxE");
        background-size: cover;
        background-position: center;
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
