<script>
import InputAutoSize from "$lib/InputAutoSize.svelte";


    let inputvalue = ""
</script>

<div class="w-72 mx-auto my-8">

    <div class="">
        <h1 class="text-center font-semibold text-lg mb-4 text-orange-600">Svelte Input Autosize</h1>
        <label for="password" class="block">Write Something</label>
        
        <InputAutoSize value={inputvalue} />
    </div>
    
    
</div>