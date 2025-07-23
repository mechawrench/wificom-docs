# Breadboard Layout

<script>
function setOptions() {
  const irLed = document.getElementById("IRLed");
  if (document.getElementById("IRMod").checked || document.getElementById("IRRaw").checked) {
    irLed.checked = true;
    irLed.disabled = true;
  } else {
    irLed.disabled = false;
  }
  var svgObject = document.getElementById("svg-object").contentDocument;
  const checkboxes = document.getElementsByClassName("showhide");
  for (let i = 0; i < checkboxes.length; i ++) {
    const checkbox = checkboxes[i];
    const layer = svgObject.getElementById("Layer" + checkbox.id);
    if (checkbox.checked) {
      layer.setAttribute("visibility", "visible");
    } else {
      layer.setAttribute("visibility", "hidden");
    }
  }
}

// Remove table of contents for more space
document.addEventListener("DOMContentLoaded", function() {
  document.getElementsByClassName("md-sidebar--secondary")[0].remove();
});
</script>
<object id="svg-object" data="/images/picow_breadboard/picow_breadboard_v2.svg" type="image/svg+xml" style="width:100%"></object>

<b>Show/Hide Sections</b><br>
<input type="checkbox" class="showhide" checked id="WiFiCom" onchange="setOptions()"><label>WiFiCom (uncheck for P-Com)</label><br>
<input type="checkbox" class="showhide" checked id="Speaker" onchange="setOptions()"><label>Speaker module</label><br>
<input type="checkbox" class="showhide" checked id="Prong" onchange="setOptions()"><label>Prong connection</label><br>
<input type="checkbox" class="showhide" checked id="Legendz" onchange="setOptions()"><label>Legendz connection</label><br>
<input type="checkbox" class="showhide" checked id="IRMod" onchange="setOptions()"><label>IR Data Link / Fusion Loader</label><br>
<input type="checkbox" class="showhide" checked id="IRRaw" onchange="setOptions()"><label>IR iC / Twin</label><br>
<input type="checkbox" class="showhide" checked disabled id="IRLed" onchange="setOptions()"><label>IR barcodes (required for other IR options)</label>

## Notes

* Bend the IR LED to point in the same direction as the sensors
* Ideally cut the front IR sensor (TSOP4838) to have shorter legs than the back one
* GND and Vcc are switched on some screens - check yours carefully - wiring these backwards will destroy the screen instantly!
* Check the pinout of your speaker module too
* The extra jumper on the top power rail is only needed if your breadboard model has gaps in the rails
* If the blue and red rails are the other way around, the important thing is which components are connected to the same one
