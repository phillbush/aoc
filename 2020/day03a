#!/usr/bin/awk -f

BEGIN           { FS = "" }
$(i + 1) == "#" { n++ }
                { i = (i + 3) % NF }
END             { print n }
