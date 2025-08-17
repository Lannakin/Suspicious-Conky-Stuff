relevent conky.conf lines:

```##################################
##          PROCESSORS          ##
##################################
${voffset 4}${font1}${color4}PROCESSOR LOAD${offset 8}${color6}${voffset -2}${hr 1}${font}
${voffset 4}${font0}${color2}CPU1 ${execpi 1 ~/.conky/ascii_bars.sh cpu 0}${offset 5}${font0}${color2}${alignr}${cpu cpu1}%${font}
${voffset 0}${font0}${color2}CPU2 ${execpi 1 ~/.conky/ascii_bars.sh cpu 1}${offset 5}${font0}${color2}${alignr}${cpu cpu2}%${font}
${voffset 0}${font0}${color2}CPU3 ${execpi 1 ~/.conky/ascii_bars.sh cpu 2}${offset 5}${font0}${color2}${alignr}${cpu cpu3}%${font}
${voffset 0}${font0}${color2}CPU4 ${execpi 1 ~/.conky/ascii_bars.sh cpu 3}${offset 5}${font0}${color2}${alignr}${cpu cpu4}%${font}
${voffset 0}${font0}${color2}CPU5 ${execpi 1 ~/.conky/ascii_bars.sh cpu 4}${offset 5}${font0}${color2}${alignr}${cpu cpu5}%${font}
${voffset 0}${font0}${color2}CPU6 ${execpi 1 ~/.conky/ascii_bars.sh cpu 5}${offset 5}${font0}${color2}${alignr}${cpu cpu6}%${font}
${voffset 0}${font0}${color2}CPU7 ${execpi 1 ~/.conky/ascii_bars.sh cpu 6}${offset 5}${font0}${color2}${alignr}${cpu cpu7}%${font}
${voffset 0}${font0}${color2}CPU8 ${execpi 1 ~/.conky/ascii_bars.sh cpu 7}${offset 5}${font0}${color2}${alignr}${cpu cpu8}%${font}
##################################
##            MEMORY            ##
##################################
${voffset 4}${font Px437 Compaq Port3:size=12}${color4}MEMORY${offset 8}${color6}${voffset -2}${hr 1}${font}
${voffset 4}${font0}${color2}RAM${goto 97}${font0}${mem}${goto 133} /${offset 5}${memmax}${alignr}${memperc}%${font}
${voffset 0}${font0}${color2}${execpi 2 ~/.conky/ascii_bars.sh memory}${font}
##################################
##           GPU LOAD           ##
##################################
${voffset 4}${font Px437 Compaq Port3:size=12}${color4}GPU LOAD${offset 8}${color6}${voffset -2}${hr 1}${font}
${voffset 4}${font0}${color2}${voffset -1}GPU0 ${font0}${offset 1}${voffset -0.5}${execpi 2 ~/.conky/ascii_bars.sh gpu}${font0}${color2}${alignr}${exec 'cat /sys/class/drm/card1/device/gpu_busy_percent'}%${font}
##################################
##           THERMALS           ##
##################################
${voffset 4}${font Px437 Compaq Port3:size=12}${color4}THERMALS${offset 8}${color6}${voffset -2}${hr 1}${font}
${voffset 4}${font0}${color2}CPU ${execpi 5 ~/.conky/ascii_bars.sh cpu_temp} ${color2}${alignr}${offset 4}${hwmon 2 temp 1}${alignr}°C${font}
${voffset 0}${font0}${color2}GPU ${execpi 5 ~/.conky/ascii_bars.sh gpu_temp} ${color2}${alignr}${offset 4}${hwmon 8 temp 2}${alignr}°C${font}```

My config is just the VinDSL config with some edits, so I feel that I probably shouldn't post the entire thing.
