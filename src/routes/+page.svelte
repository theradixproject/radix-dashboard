<script lang="ts">
    import Button from "$lib/components/Button.svelte";
	import { redirect } from "@sveltejs/kit";
</script>

<div class="grid grid-cols-1 grid-rows-1 place-items-center">
    <h1 class="text-3xl">Radix Project Dashboard</h1>
    <Button onclick={() => { console.log("redirect"); redirect(307, "/new_project") }}>
        New Project
    </Button>
</div>