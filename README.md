# 1keySSR

Original Designer is here:
https://github.com/ToyoDAdoubi/doubi#ssrsh
\p
Here is my slightly imporved script for building basic SSR server in Bandwagon/Goolge Cloud and a backup site in case of the GFW (since doub's io is already hangup in Dec.2018)
\p
To use the 1key SSR for personal purpose just copy and run the following 
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh

Debian 7+/Ubuntu 16+ already set BBR as default TCP control algorithm, there is no need to extra operate the bbr.sh
For those who need a second check or installation of BBR run (typically Debian 6/Ubuntu 14):
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh
Verification of a successfull BBR control would be realized through test the following command with root power:
sysctl net.ipv4.tcp_congestion_control
If you get something like:
net.ipv4.tcp_congestion_control = bbr
Then the BBR is already activated.

Another version of scripte to realise ss-go (do check its not ssr):
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/ss-go.sh && chmod +x ss-go.sh && bash ss-go.sh



