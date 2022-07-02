<script lang="ts">
    import FeedbackList from './components/FeedbackList.svelte'
    let feedback = [
        {
            id: 1,
            rating: 10,
            text: 'Eiusmod id nulla pariatur ut ut non cupidatat excepteur officia eu. Duis tempor anim anim mollit et aute. Sit aute cupidatat duis deserunt. Excepteur velit sunt quis nostrud. Et pariatur aliqua eiusmod magna sunt officia nisi. Nisi ea officia ea nulla.',
        },
        {
            id: 2,
            rating: 8,
            text: 'Lorem cillum aliqua nulla ut Lorem nulla elit aliquip do. Mollit labore ullamco tempor ipsum eu et duis proident excepteur exercitation labore magna. Aliquip nostrud velit anim mollit culpa dolore ullamco nostrud non ad sunt.',
        },
        {
            id: 3,
            rating: 9,
            text: 'Voluptate aliqua consequat sunt in do officia Lorem minim enim irure anim laborum ullamco. Ad ipsum adipisicing ipsum deserunt proident minim fugiat. Ipsum elit nulla culpa Lorem non id. Ipsum voluptate ullamco ad id sunt officia enim amet culpa incididunt deserunt. Labore consectetur commodo sunt excepteur ea Lorem dolor magna id eu in duis laboris Lorem. Ad in officia anim eu. Ut cupidatat laborum elit aute commodo exercitation aute excepteur voluptate cillum irure.',
        },
    ]
</script>

<main class="max-w-xl my-6 mx-auto px-5">
    <FeedbackList {feedback} />
</main>
