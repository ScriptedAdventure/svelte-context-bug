<script>
    import { getContext } from "svelte";
	import { afterNavigate } from '$app/navigation';

    afterNavigate(() => {
        const store = getContext("test").store;
        store.set(1);
    });
</script>

{getContext("test").$store}

<a href="/">Go to other page</a>
