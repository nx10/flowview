<script lang="ts">
    export let title = '';
    export let free_height: boolean = false;
</script>

<div class="rounded-md border shadow-md p-2 m-2 basis-1/2 grow-0 overflow-auto">
    <h2 class="font-medium mb-1">{title}</h2>
    <div class="{free_height ? '': 'max-h-80 overflow-auto'}">
        <slot/>
    </div>
</div>