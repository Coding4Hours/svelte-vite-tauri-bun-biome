<script>
    /** @type {(action: string, frame: string) => void} */
    let chemicalAction;
</script>

<input autofocus spellcheck="false" autocomplete="off" id="search" data-frame="web" data-auto-https data-search-engine="https://www.google.com/search?q=%s" placeholder="Search or Enter a URL" is="chemical-input">
<section id="controls" is="chemical-controls">
    <button onclick={() => chemicalAction('back', 'web')}>Back</button>
    <button onclick={() => chemicalAction('forward', 'web')}>Forward</button>
    <button onclick={() => chemicalAction('reload', 'web')}>Reload</button>
    <button onclick={() => chemicalAction('close', 'web')}>Close</button>
</section>
<iframe title="proxy stuff" id="web" data-controls="controls" is="chemical-iframe"></iframe>