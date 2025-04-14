<script>
    import { goto } from "$app/navigation";
    function next() {
        goto("/");
    }
    function previous() {
        goto("/projects");
    }
</script>

<header class="flex justify-center align-items-start text-[3rem]">
    <h1 class="bg-blue-200 rounded-2xl p-2 mt-5 mb-10 font-extrabold">
        <u>Mes infos </u>
    </h1>
</header>
<section class="flex flex-col">
    <div
        class="flex justify-center items-center text-center text-[2rem] font-bold"
    >
        <p>
            sur cette page vous pouvez me contacter <br />
            et avoir des information a propo de moi
        </p>
    </div>
</section>
<footer class="flex justify-center align-items-end flex-col font-bold">
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
    <div class="flex flex-col items-center " target="_blank">
        <form
            action="https://formspree.io/f/xnnpwebz"
            method="POST"
            class="flex flex-col"
            target="_blank"
        >
        <div class="flex flex-row">
            <label class="p-10 bg-green-300 rounded-tl-4xl text-center">
                <u>↓votre email↓<br>
                <textarea type="email" name="email" target="_blank" ></textarea>
            </label>
            <label class="p-10 bg-green-300 rounded-tr-4xl text-center">
                <u>↓votre message↓<br>
                <textarea name="message" target="_blank"></textarea>
            </label>
        </div>
            <button type="submit" class="rounded-b-4xl bg-amber-500 hover:bg-amber-200" target="_blank">Send</button>
        </form>
    </div>
</footer>

<style>
</style>
