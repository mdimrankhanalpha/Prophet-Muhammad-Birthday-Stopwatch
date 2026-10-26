SEERAH — ETERNAL TIME
=====================

Open index.html in a modern browser. The page is a lightweight, responsive,
six-counter elapsed-time display.

Important accuracy notes:
- The historical reference is intentionally marked approximate: 571 CE,
  April 20 (disputed), 06:00 AM (speculative). It is not an exact verified
  birth timestamp.
- The page obtains UTC from an internet time API and never falls back to the
  device date/time. If both time services are unavailable, it shows dashes and
  waits for synchronization.
- Once synchronized, it advances using the browser's monotonic performance
  timer, so changing the device clock does not change the running count.
- Browser JavaScript cannot guarantee a timer survives every possible event
  forever: closing the page, browser/OS termination, power loss, or unavailable
  internet can interrupt display updates. It re-synchronizes when reopened.
- Nanosecond figures are a calculated display, not true nanosecond hardware
  precision.
- Year/month/day decomposition is a duration-style approximation because the
  chosen historic date and time are uncertain.

For GitHub Pages: upload index.html to the repository root and enable Pages.
