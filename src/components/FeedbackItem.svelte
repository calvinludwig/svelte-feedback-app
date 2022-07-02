<script lang="ts">
    import Card from './Card.svelte'
    export let item
</script>

<Card>
    <div
        class="num-display absolute w-12 h-12 bg-rose-400 text-whit rounded-full text-center p-2 text-lg font-semibold border-2 border-solid border-white"
    >
        {item.rating}
    </div>
    <div class="absolute top-2 right-3 cursor-pointer ">X</div>
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
