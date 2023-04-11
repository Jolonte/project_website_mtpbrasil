<script lang="ts">
    import TheButton from "./TheButton.svelte";


</script>

<form class="flex flex-col items-center gap-[2rem]" action="POST" >
    <input class="w-full py-[0.625rem] px-[1.125rem] rounded-[0.938rem]" placeholder="Nome e sobrenome*" type="text" name="Nome">
    <input class="w-full py-[0.625rem] px-[1.125rem] rounded-[0.938rem]" placeholder="E-mail*" type="text" name="Email">
    <input class="w-full py-[0.625rem] px-[1.125rem] rounded-[0.938rem]" placeholder="Número de celular" type="text" name="Telefone">
    <textarea class="w-full py-[0.625rem] px-[1.125rem] rounded-[0.938rem] h-40 resize-none" placeholder="Como podemos ajudá-lo?*" name="Consulta"></textarea>
    <TheButton propTitle="Enviar" />
</form>