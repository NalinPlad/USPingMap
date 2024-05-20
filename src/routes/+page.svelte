<script>

let main_button = false;

function toggleMain() {
    main_button = !main_button;
    // alert(1)
}

</script>

<svelte:window
    on:keydown={toggleMain}
    on:keyup={toggleMain}
    style="{main_button ? 'background-color: red' : 'background-color: blue'}"
/>


<input
on:keydown={main_button = true}
on:keyup={main_button = false}
style="{main_button ? 'background-color: red' : 'background-color: blue'}"
/>