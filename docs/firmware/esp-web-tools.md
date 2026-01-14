---
icon: lucide/wrench
---

# ESP Web Tools
# Installation

You can use the options below to install the factory firmware directly to your device via USB from the browser. Note
this has already been done from the factory. You only need to do this if you're trying to start fresh, or grab the
latest updates.

You can also use it to get device info, check which version is installed, view logs, change Wi-Fi, or add to Home
Assistant.

## Select Device

<!-- Bed Presence Mk1 (Default Device) -->
<div class="form-check">
    <input class="form-check-input" type="radio" name="deviceType" value="bed-presence-mk1" id="deviceType1" checked>
    <label class="form-check-label" for="deviceType1">
        Bed Presence Mk1
    </label>
</div>

<!-- Add next device -->
<!-- <div class="form-check"> -->
<!--     <input class="form-check-input" type="radio" name="deviceType" value="test" id="deviceType2"> -->
<!--     <label class="form-check-label" for="deviceType2"> -->
<!--         Test Device -->
<!--     </label> -->
<!-- </div> -->

<p class="button-row" align="center">
  <esp-web-install-button
    <!-- manifest="https://docs.elevatedsensors.com/firmware/bed-presence-mk1/latest/manifest.json" -->
    manifest="https://elevatedsensorsdocs.netlify.app/products/bed-presence-mk1/manifest.json"
  >
    <button slot="activate" class="md-button md-button--primary">
      Connect
    </button>
    <span slot="unsupported">
      Your browser does not support installing things on ESP devices. Use Google Chrome or Microsoft Edge.
    </span>
    <span slot="not-allowed">
      You can only install ESP devices on HTTPS websites or on the localhost.
    </span>
  </esp-web-install-button>
</p>

<!-- ESPWebTools script -->
<script type="module" src="https://unpkg.com/esp-web-tools@10/dist/web/install-button.js?module"></script>

<!-- Update manifest based on selected device -->
<script>
  <!-- const manifestBase = "https://docs.elevatedsensors.com/firmware/"; -->
  const manifestBase = "https://elevatedsensorsdocs.netlify.app/firmware/";

  document.querySelectorAll('input[name="deviceType"]').forEach(radio =>
    radio.addEventListener("change", () => {
      const button = document.querySelector('esp-web-install-button');
      button.manifest = `${manifestBase}${radio.value}/latest/manifest.json`;
    }
  ));
</script>
