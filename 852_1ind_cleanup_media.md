rule "adjust first indicator of 852 for film & video materials"
when
	(exists "852.b.FILM")
then 
	changeFirstIndicator "852" to "8" if (exists "852.{1,*}")
	changeFirstIndicator "852" to "8" if (exists "852.{0,*}")
end