#!/usr/bin/awk -f

BEGIN                { FS = ""; ai = bi = ci = di = ei = 1 }
$ai == "#"           { an++ }
$bi == "#"           { bn++ }
$ci == "#"           { cn++ }
$di == "#"           { dn++ }
$ei == "#" && NR % 2 { en++ }
                     { ai = ((ai + 0) % NF) + 1 }
                     { bi = ((bi + 2) % NF) + 1 }
                     { ci = ((ci + 4) % NF) + 1 }
                     { di = ((di + 6) % NF) + 1 }
NR % 2               { ei = ((ei + 0) % NF) + 1 }
END                  { print an * bn * cn * dn * en }
