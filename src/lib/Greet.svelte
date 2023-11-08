<script>
  import { invoke } from '@tauri-apps/api/tauri'

  let name = ''
  let greetMsg = ''

  async function greet() {
    console.log("Hiiii");
    greetMsg = await invoke('greet', { name })
  }
</script>

<div>

<input type="text" placeholder="Type here" class="input input-bordered w-full max-w-xs" bind:value="{name}" />
  <button on:click="{greet}">Greet</button>
  <p>{greetMsg}</p>
  <div> 
    <button class="btn">Hello daisyUI</button>
    <input type="checkbox" checked="checked" class="checkbox" />
</div>
</div>
