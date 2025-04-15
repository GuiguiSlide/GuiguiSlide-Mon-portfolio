<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/");
    }
    function previous() {
        goto("/projects");
    }
</script>

<div class="bg-[rgba(255,255,255,0.5)] rounded-4xl m-20 fade">
    <header class="flex justify-center align-items-start text-[3rem] fade">
        <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold fade">
            <u>Mes infos</u>
            <!-- ❌ espace inutile -->
        </h1>
    </header>

    <section class="flex flex-col fade">
        <div
            class="flex justify-center items-center text-center text-[2rem] font-bold fade"
        >
            <p>
                Sur cette page, vous pouvez me contacter<br />
                et obtenir des <u>informations à propos de moi</u>.<br /><br />
                <!-- ❌ "information a propo" => ✅ "informations à propos" -->
            </p>
        </div>
    </section>

    <div class="flex flex-row justify-around">
        <div class="flex flex-col items-center justify-center" target="_blank">
            <form
                action="https://formspree.io/f/xnnpwebz"
                method="POST"
                class="flex flex-col"
                target="_blank"
            >
                <div class="flex flex-row">
                    <label
                        class="p-10 bg-green-300 rounded-tl-4xl text-center w-[50%]"
                    >
                        <u>
                            ↓Votre email↓<br />
                            <textarea type="email" name="email" class="w-[50%]"
                            ></textarea>
                        </u>
                    </label>
                    <label
                        class="p-10 bg-green-300 rounded-tr-4xl text-center w-[50%]"
                    >
                        <u>
                            ↓Votre message↓<br />
                            <textarea name="message" class="w-[50%]"></textarea>
                        </u>
                    </label>
                </div>
                <button
                    type="submit"
                    class="rounded-b-4xl bg-amber-500 hover:bg-amber-200 w-[100%]"
                >
                    Envoyer <!-- ✅ "Send" → français pour cohérence -->
                </button>
            </form>
        </div>

        <div class="font-bold">
            Contact : 07 69 36 53 11<br />
            Mail : guillaum29280.fr@gmail.com<br />
            <!-- ✅ espace après ":" -->
        </div>
    </div>

    <footer class="flex justify-center align-items-end flex-col font-bold">
        <div
            class="flex flex-row text-center justify-center p-10 text-[2.5rem]"
        >
            <button
                onclick={previous}
                class="bg-red-900 rounded-4xl p-5 mr-5 mt-30 min-w-[15rem] font-extrabold hover:bg-red-700 z-10"
            >
                ← Précédent <!-- ✅ majuscule -->
            </button>
            <button
                onclick={next}
                class="bg-green-900 rounded-4xl p-5 ml-5 mt-30 min-w-[15rem] font-extrabold hover:bg-green-700 z-10"
            >
                Retour → <!-- ❌ "retour←|" => ✅ "Retour →" -->
            </button>
        </div>
    </footer>
</div>

<style>
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
