Debian 12 (bookworm) has a very old release of the snowflake-proxy (2.5.1) 

I created a new deb file with a few enhancments compared to the old
snowflake-proxy that Debian provides.

Version : 2.9.2 (very new)
manual page 1 (snowflake-proxy) : I did add the missing options, that were missing in the man page from Debian 
user : The old Debian snowflake-proxy (2.5.2) have used root for running the proxy.The new Deb file is using a 
a other user to run the proxy. As long I did running the old proxy (2.5.1) with user root, I had no connection.
After compiling snwoflake-proxy 2.9.2 as normal user and running as user snowflake I had connections on my server.

To build the software you ned golang-go 1.2.1 or higher ...
Debian provides 1.91 ... so you have to install a later golang-go

https://www.linuxcapable.com/how-to-install-golang-go-on-debian-linux/
create a new user snowflake 

su snowflake 
git clone https://git.torproject.org/pluggable-transports/snowflake.git


cd snowflake/proxy



     
