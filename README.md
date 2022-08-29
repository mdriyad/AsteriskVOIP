# AsteriskVOIP

This repor contains the .conf files required to properly setup the asterisk voip server in Ubuntu.

Can call but no voice issue
https://stackoverflow.com/questions/27230993/asterisk-can-call-and-answer-but-no-voice-or-video
Resolved ! I had to configure externip=my.external.ip in sip.conf, because I'm running asterisk behind a NAT !
I also added h263 codec to make video work, and added videosupport=yes in sip.conf
