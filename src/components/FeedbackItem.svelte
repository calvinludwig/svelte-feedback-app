<script lang="ts">
    import { createEventDispatcher } from 'svelte'
    import Card from './Card.svelte'

    export let item

    const dispatch = createEventDispatcher()
    const handleDelete = (itemId) => {
        dispatch('delete-feedback', itemId)
    }
</script>

<Card>
    <div
        class="num-display absolute w-12 h-12 bg-rose-400 text-whit rounded-full text-center p-2 text-lg font-semibold border-2 border-solid border-white"
    >
        {item.rating}
    </div>
    <button
        class="absolute top-2 right-3 cursor-pointer"
        on:click={() => handleDelete(item.id)}>X</button
    >
    <p>
        {item.text}
    </p>
</Card>

<style>
    .num-display {
        top: -1rem;
        left: -1rem;
    }
</style>
