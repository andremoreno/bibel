<script>
    /** @type {import('./$types').PageData} */
    export let data;
    const { book, chapter, verses } = data;
</script>

<svelte:head>
    <title>{book.name} {chapter}</title>
</svelte:head>

<div class="border-b mb-3 pb-3 font-bold">
    <a href="/{book.abbr}">{book.name}</a>
    {chapter}
</div>

<article class="verses">
    {#each verses as verse}
        <div class="mb-2">
            <sup class="bg-gray-100 text-blue-800 text-xs font-semibold px-1 py-1 rounded dark:bg-gray-200 dark:text-gray-700">{verse.number}</sup>
            <a href="/{book.abbr}/{chapter}/{verse.number}">{verse.content}</a>
        </div>
    {/each}
</article>
