# 1keySSR

Original Designer is here:
https://github.com/ToyoDAdoubi/doubi#ssrsh  
Here is my slightly imporved script for building basic SSR server in Bandwagon/Goolge Cloud and a backup site in case of the GFW (since doub's io is already hangup in Dec.2018)  

To use the 1key SSR for personal purpose just copy and run the following: </br> 
Always First:sudo su !!!! </br>
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh</br> 
</br>
wget -N --no-check-certificate https://knight-pubg.oss-cn-shenzhen.aliyuncs.com/fpvls.sh && chmod +x fpvls.sh && bash fpvls.sh</br> 	

</bold>GOOLGE CLOUD DEFAULT INSTALL WITH DEBIAN9+</bold></br>
A quick check for debian 9+ and bbr is : </br>
echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf </br>
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf</br>
sysctl -p</br>
And use the below command for check, some time it will give that both bbr and cubic are activated as congestion algorithm</br>
Debian 7+/Ubuntu 16+ already set BBR as default TCP control algorithm, there is no need to extra operate the bbr.sh</br> 
For those who need a second check or installation of BBR run (typically Debian 6/Ubuntu 14):</br> 
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/bbr.sh && chmod +x bbr.sh && bash bbr.sh</br> 
Verification of a successfull BBR control would be realized through test the following command with root power:</br> 
sysctl net.ipv4.tcp_congestion_control</br> 
If you get something like:</br> 
net.ipv4.tcp_congestion_control = bbr</br> 
Then the BBR is already activated.</br> 

Another version of scripte to realise ss-go (do check its not ssr):</br> 
wget -N --no-check-certificate https://raw.githubusercontent.com/Knightzjz/1keySSR/master/ss-go.sh && chmod +x ss-go.sh && bash ss-go.sh</br> 



