rule "852 second indicator 0"
when
   (exists "852.{0,*}")
then
   set indication."true"
end