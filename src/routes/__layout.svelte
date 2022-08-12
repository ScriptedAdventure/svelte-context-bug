<script>
    import { setContext } from "svelte";
    import { writable } from "svelte/store";

    setContext("test", {
        store: writable(0),
    });
</script>

<slot />
