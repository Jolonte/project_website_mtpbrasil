<script>
    import TheButton from "../components/TheButton.svelte";
</script>

<header class="flex flex-col items-center pt-[3.438rem] px-[12.25rem] h-screen bg-[#dfe6e9]">
    <nav class="flex w-[57.313rem]">
        <img src="/mtp_logo.png" alt="Logo MTP">
        <ul class="flex w-full justify-center gap-[2.313rem] uppercase">
            <li>Sobre a MTP</li>
            <li>Serviços</li>
            <li>Setores</li>
            <li>Cases</li>
            <li>Carreira</li>
            <li>Blog</li>
        </ul>
        <!-- imagem responsável por manter padding equilibrado -->
        <img class="opacity-0" src="/mtp_logo.png" alt="Logo MTP">
    </nav>
    <!-- Hero Section -->
    <div class="flex flex-col items-center gap-[1.063rem] pt-[2.688rem]">
        <h1 class="font-bold text-5xl text-center text-[#2f2e41]">Uma empresa com 25 anos de história, em constante <span class="text-blue-600">crescimento</span></h1>
        <div class="pt-[1.5rem]">
            <ul class="flex gap-[2.5rem] w-full justify-center">
                <li class="flex items-center gap-[0.5rem]">
                    <i class="material-symbols-outlined text-blue-600">done</i>
                    Satisfação do cliente
                </li>
                <li class="flex items-center gap-[0.5rem]">
                    <i class="material-symbols-outlined text-blue-600">done</i>
                    Soluções personalizadas
                </li>
                <li class="flex items-center gap-[0.5rem]">
                    <i class="material-symbols-outlined text-blue-600">done</i>
                    Expertise comprovada
                </li>
            </ul>
        </div>
        <TheButton propTitle="Mais informações" />
        <img class="mt-[3rem] w-[35rem]" src="/hero_image.svg" alt="Imagem: Trabalho em equipe">
    </div>
</header>
