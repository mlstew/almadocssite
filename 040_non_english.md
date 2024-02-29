rule "non-English 040"
when
	(exists "040" AND not exists "040.b.eng")
then
	set indication."true"
end