The file frenchs.sh is an auxiliary script to Heinz and Suls.

If using Suls to generate bouquets, and you've filled in the parameter

"Support info file"

in Heinz to point to

"/tmp/heinz.inf"

this script will look for said file to mark all catchup supporting channels
with a

"!!!"

suffix on the channel name.

NOTE: if you don't use exclamation mark(s) as the suffix, the channel
renaming will break the proper picons display.


The script can be run manually, but it's better if ran via cron, as Suls
generally also runs periodically. A crontab line to run it every 5 minutes is
as such:

*/5 * * * * /usr/lib/enigma2/python/Plugins/Extensions/Heinz/frenchs.sh pmc

NOTE: the provider name is provided as the first argument of the script.
