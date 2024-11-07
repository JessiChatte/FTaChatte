<script lang="ts">
    import "../app.css";
    import { ModeWatcher, toggleMode } from "mode-watcher";
    import {Button} from "$lib/components/ui/button";
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
</script>
<ModeWatcher />
<Button onclick={toggleMode}>Theme</Button>
{@render children?.()}
