rule "HathiTrust information for 583"
priority 2
when
TRUE
then
addField "ZZZ.{ ,-}.a.Committed to retain"
addSubField "ZZZ.c.20170930"
addSubField "ZZZ.d.20421231"
addSubField "ZZZ.f.HathiTrust Shared Print Program"
addSubField "ZZZ.2.pda"
addSubField "ZZZ.5.DeU"
end

rule "adjust ZZZ to 583"
priority 1
when
TRUE
then
changeField "ZZZ" to "583"
end

# notes about field 583 blank,- $a Committed to retain $c 20170930 $d 20421231 $f HathiTrust Shared Print Program $2 pda $5 DeU