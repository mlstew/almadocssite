rule "583 with Mark step information"
when
	(exists "583.a.*Mark*")
then
	set indication."true"
end