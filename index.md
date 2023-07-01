---
layout: default
title: Resident Break Calendar
order: 1
---

# [Click here to add your free days!](https://forms.gle/DJogHaLU7Mrzd4U2A)

<a href="https://forms.gle/DJogHaLU7Mrzd4U2A" class="fab">+</a>
<style>
  .fab {
  border: none;
  height: 56px;
  width: 56px;
  background-color: hotpink;
  border-radius: 16px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 24px;
  color: white;
  box-shadow: 0 0 5px rgba(0, 0, 0, .25);
}
</style>

---

<div id="observablehq-searchInput-7d891de1"></div>

---

<div id="observablehq-calendarEl-7d891de1"></div>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@observablehq/inspector@5/dist/inspector.css">
<script type="module">
import {Runtime, Inspector} from "https://cdn.jsdelivr.net/npm/@observablehq/runtime@5/dist/runtime.js";
import define from "https://api.observablehq.com/d/d379ad992bc21262@201.js?v=3";
const runtime = new Runtime()
const main = runtime.module(define, name => {
  if (name === "searchInput") return new Inspector(document.querySelector("#observablehq-searchInput-7d891de1"));
  if (name === "calendarEl") return new Inspector(document.querySelector("#observablehq-calendarEl-7d891de1"));
  return ["calendar","handleSearch","debouncedHandleSearch"].includes(name);
});
main.redefine("GOOGLE_SHEETS_API_KEY", "AIzaSyDln9ZScDNAYGPm-ueXLEf6W7zlbNI9qN8")
</script>
