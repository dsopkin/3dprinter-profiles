# Octoprint Custom scripts

## After print job is cancelled

; disable motors
M84

;disable all heaters
{% snippet 'disable_hotends' %}
{% snippet 'disable_bed' %}
;disable fan
M106 S0

; move up 40mm
G1 Z50 F3600