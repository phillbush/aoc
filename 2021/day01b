#!/usr/bin/awk -f

                                 { c = NR % 4 }
                                 { for (i = 0; i < 4; i++) if (i != c) a[i] += $0 }
NR > 3 && a[(NR + 1) % 4] > a[c] { m++ }
                                 { a[c] = 0 }
END                              { print m }
