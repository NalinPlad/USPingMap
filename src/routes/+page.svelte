<script>

let main_button = false;

</script>

<svelte:window
    on:keydown={main_button = true}
    on:keyup={main_button = false}
/>

