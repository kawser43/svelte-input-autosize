# svelte-input-autosize

![Gif](https://raw.githubusercontent.com/kawser43/svelte-input-autosize/main/static/demo.gif)

## Install

```
$ npm install svelte-input-autosize
```

## Usage

```
<script>
    import InputAutoSize from 'svelte-input-autosize'
    let inputvalue = ""
</script>

<div class="w-full mx-auto my-8">
    <div class="">
        <h1 class="text-center font-semibold text-lg mb-4 text-orange-600">Svelte Input Autosize</h1>
        <label for="password" class="block">Write Something</label>

        <InputAutoSize value={inputvalue} />
    </div>
</div>
```
