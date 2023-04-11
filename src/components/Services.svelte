<script lang="ts">
    // props
    export let propIcon: string;
    export let propTitle: string;
    export let propDesc: string;
</script>

<div class="flex flex-col gap-[1.438rem]">
    <i class="material-symbols-outlined text-blue-600 text-7xl">{propIcon}</i>
    <div class="flex flex-col gap-[0.813rem]">
        <h3 class="font-bold text-2xl">{propTitle}</h3>
        <p class="w-[25rem]">{propDesc}</p>
    </div>
</div>