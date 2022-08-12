<script>
    import { getContext } from "svelte";
    import { afterNavigate } from "$app/navigation";

    afterNavigate(() => {
        const store = getContext("test").store;
        store.set(2);
    });
</script>

{getContext("test").$store}

<a href="/">Go to other page</a>
