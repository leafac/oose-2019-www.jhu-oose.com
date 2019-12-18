<span id="time"></span> minutes left.

<!-- Write here anything else you want to show students, for example, clarifications during an exam. -->

<script>
const endAt = "2019-11-20T14:45-05:00";
function tick() {
  document.querySelector("#time").innerText = Math.ceil((new Date(endAt) - new Date()) / 60000);
}

setInterval(tick, 1000);
</script>
