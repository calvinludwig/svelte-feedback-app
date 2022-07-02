<script>
    import Card from './Card.svelte'

    let btnDisabled = false
</script>

<Card>
    <header>
        <h2>How would you rate your service with us?</h2>
    </header>
    <form action="">
        <div class="relative">
            <input
                class="py-2 px-4 w-full bg-slate-100 border-2 border-red-500"
                type="text"
                placeholder="Tell us something that keeps you coming back"
            />
            <button
                class="absolute right-0 text-white rounded-md bg-slate-800 py-2 px-4 cursor-pointer hover:bg-slate-700 active:bg-slate-900 disabled:bg-slate-300 disabled:text-slate-500 disabled:cursor-default"
                disabled={btnDisabled}
                type="submit">Send</button
            >
        </div>
    </form>
</Card>
