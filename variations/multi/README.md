= Casual Tux Hawaiian Multi =

Casual Tux Hawaiian is wearing a shirt made with the Black Hawaiian pattern.

The Black Hawaiian pattern has Multi1 and Multi2.  For Casual Tux Hawaiian I decided to make things less confusing and just pick one, and the one I chose was Multi2.

I figured there might be times when I would want the penguin matching the pattern, so I kept both in svg format only.

== Steps ==

How to change CasualTux-Hawaiian-Multi.svg to CasualTux-Hawaiian-Multi1.svg

 * cp CasualTux-Hawaiian-Multi.svg CasualTux-Hawaiian-Multi1.svg
 * sed -i "s/Multi/Multi1/" CasualTux-Hawaiian-Multi1.svg
 * grep -A 1 -B 1 linearGradient5397 CasualTux-Hawaiian-Multi1.svg | grep radial | awk -F'"' '{print $2}'| while read line; do echo $line ; sed -i "s/$line);fill-opacity:1;fill-rule:nonzero;stroke:#cc0022;/$line);fill-opacity:1;fill-rule:nonzero;stroke:#ffffff;/" CasualTux-Hawaiian-Multi1.svg ; done
 * grep -A 1 -B 1 linearGradient6719 CasualTux-Hawaiian-Multi1.svg | grep radial | awk -F'"' '{print $2}'| while read line; do echo $line ; sed -i "s/$line);fill-opacity:1;fill-rule:nonzero;stroke:#ffffff;/$line);fill-opacity:1;fill-rule:nonzero;stroke:#cc0022;/" CasualTux-Hawaiian-Multi1.svg ; done
