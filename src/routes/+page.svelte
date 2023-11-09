<script lang="ts">
    import Greet from '../lib/Greet.svelte';
    import Icon from '@iconify/svelte';
    import '../app.css';

    export const prerender = true
    export const ssr = false
</script>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<Icon icon="mdi-light:home" />
<Greet /> 
