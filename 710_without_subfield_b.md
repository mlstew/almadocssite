rule "710 without subfield b"
when
	( (exists "710.{-,-}.*") AND (not exists "710.{-,-}.b.*") )
then
	set indication."true"
end