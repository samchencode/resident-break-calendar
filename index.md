---
layout: page
title: Resident Break Calendar
order: 1
---

<div id="observablehq-searchInput-1e1dd4b7"></div>
<div id="observablehq-viewof-calendar-1e1dd4b7"></div>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@observablehq/inspector@5/dist/inspector.css">
<script type="module">
    import { Runtime, Inspector } from "https://cdn.jsdelivr.net/npm/@observablehq/runtime@5/dist/runtime.js";
    import define from "https://api.observablehq.com/d/d379ad992bc21262@160.js?v=3";
    
    const runtime = new Runtime()
    const main = runtime.module(define, name => {
        if (name === "searchInput") return new Inspector(document.querySelector("#observablehq-searchInput-1e1dd4b7"));
        if (name === "viewof calendar") return new Inspector(document.querySelector("#observablehq-viewof-calendar-1e1dd4b7"));
        return ["handleSearch", "debouncedHandleSearch"].includes(name);
    });
    main.redefine("GOOGLE_SHEETS_API_KEY", "AIzaSyDln9ZScDNAYGPm-ueXLEf6W7zlbNI9qN8")
</script>
