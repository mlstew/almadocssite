rule "correction of 710 indicators based on presence or absence of $b"
priority 2
when
exists "710.{-,-}"
then
changeFirstIndicator "710" to "1" if (exists "710.b.*")
end

rule "change the others"
priority 1
when
exists "710.{-,-}"
then
changeFirstIndicator "710" to "2" if (exists "710.{-,-}")
end