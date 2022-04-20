<script>
  import "./app.css";
  import { onMount } from "svelte";
  export let value = "";
  let dynamic_width = 1

  let input_field;
  onMount(async () => {
    input_field = document.getElementById("dynamic_input")
    input_field.addEventListener("keyup", calculateWidth);
    return () => input_field.removeEventListener("keydown", calculateWidth);
  });

  const calculateWidth = () => {
    if (input_field == undefined) {
      input_field = document.getElementById("dynamic_input")
    }

    const total_char = value.toString().length;
    if (total_char > 0) {
      dynamic_width = total_char
    } else {
      dynamic_width = 1
    }
  };
</script>

<div class="my-2">
  <input id="dynamic_input" type="text" bind:value class="border border-gray-600 rounded-sm" style={`width: ${dynamic_width}ch`} />
</div>