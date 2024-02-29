rule "710 check for subfield b"
when
	exists "710.{-,-}.b.*"
then
	set indication."true"
end