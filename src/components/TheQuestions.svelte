<script lang="ts">
    export let propTitle: string;
</script>

<div class="flex flex-col gap-[0.5rem]">
    <div class="flex justify-between">
        <h3 class="font-bold text-xl">{propTitle}</h3>
        <i class="material-symbols-outlined text-blue-600 text-4xl">expand_more</i>
    </div>
    <hr class="border-b-[0.1rem] border-blue-600">
</div>