<script lang="ts">
    import "../app.css";
    import { ModeWatcher, toggleMode } from "mode-watcher";
    import {Button} from "$components/ui/button";
</script>
<ModeWatcher />
<Button on:click={toggleMode}>Theme</Button>
<slot></slot>
