<script lang="ts">
    import Header from "./lib/TheHeader.svelte";
    import Main from "./lib/TheMain.svelte";
</script>

<div class="flex flex-col">
    <Header />
    <Main />
    <footer class="flex flex-col items-center py-[9.5rem] px-[12.25rem] gap-[4rem] bg-[#2f2e41]">
        <div class="flex justify-center w-full gap-[1rem]">
            <p class="uppercase text-white text-lg">Sobre</p>
            <p class="uppercase text-white text-lg">Serviços</p>
            <p class="uppercase text-white text-lg">Setores</p>
            <p class="uppercase text-white text-lg">Talento</p>
            <p class="uppercase text-white text-lg">Formação</p>
            <p class="uppercase text-white text-lg">Fornecedores</p>
            <p class="uppercase text-white text-lg">Blog</p>
            <p class="uppercase text-white text-lg">Políticas</p>
            <p class="uppercase text-white text-lg">Contato</p>
        </div>
        <img src="/mtp_banner.png" alt="">
    </footer>
</div>
