<script lang="ts">
    export let onclick: (e:any) => void;
</script>

<button on:click={onclick} class="bg-black border-purple-500 border-4 p-10 pl-20 pr-20 m-5">
    <main class="text-purple-500 font-bold">
        <slot />
    </main>
</button>