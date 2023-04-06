# tcptools
***Using ping for three popular websites***

**www.amazon.com**

1. IP - Reply from 205.251.242.103. The IP did not change throughout the 4 pings. 
2. Sent 4 packets and received 4 for a 0% loss. The minimum time was 84ms, maximum time was 90ms, and average time was 85ms. 
3. Each ping sent 32 bytes and had a time to live of 218.

**www.google.com**

1. IP - 142.251.33.110. The IP did not change throughout the 4 pings. 
2. Sent 4 packets and received 4 packets for a 0% loss. The minimum time was 17ms, maximum time was 29ms and the average time to complete the ping was 21ms. 
3. Each ping sent 32 bytes and had a time to live of 56.

**www.microsoft.com**

1. IP - Ping was sent to www.microsoft.com. The reply was sent from e13678.dscb.akamaiedge.net (23.45.229.117). IP did not change throughout the 4 pings. 
2. The ping sent 4 packets and received 4 packets for a 0% loss. The minimum time was 21ms, maximum response time was 36ms, and the average response time was 27ms. 
3. Each ping sent 32 bytes and had a time to live of 57.

***tracert for three popular websites***

**www.amazon.com**

1.Targer Server IP - server-18-172-169-208.sea73.r.cloudfront.net [18.172.169.208]
2.17 hops were required to reach the target
3. ISP - the ISP is Comcast as that name showed up in several of the hops. e.g.  be-501-arsc1.seattle.wa.seattle.comcast.net
4. Class of IPs - The tracert began with my default gateway of 192.168.1.1 which is a Class C address. The next hop is a 10.1.10.1 address, Class A, followed by a 100.92.123.67, also Class A. Followed by 6 hops, all of which contain comcast addresses and all within the class A address range. The request then times out for 5 hops before arriving at 15.230.247.0, a class A. Finally arriving at the destination 18.172.16.208, a Class A. Overall once leaving my class C default gateway, the hops consisted of only Class A addresses.

**www.google.com**

1. Target Server IP - 172.217.14.196 sea30s01-in-f4.1e100.net
2. 11 Hops were required to reach the target. 
3. ISP - the ISP is comcast. e.g. po-323-406-rur302.seattle.wa.seattle.comcast.net. 
4. Again the tracert began with my default gateway of 192.168.1.1, a class C address. Following the same path, heading to 10.1.10.1, class A, followed by 100.92.123.67, class A. Follows with 5 hops, all comcast addresses and all class A. Then hits 3 Class B addresses before reaching the destination at 172.217.14.196.

**www.microsoft.com**

1. Target Server IP - e13678.dscb.akamaiedge.net [23.44.161.156]
2. 13 Hops were required to reach Microsoft. 
3. ISP - the ISP is Comcast. 
4. The tracert begins with my IP of 192.168.1.1, a class C. Then follows the same path, 10.1.10.1 and then 100.92.123.67, both class A's. Then hits 9 class A's in a row, all comcast addresses. Finally reaching the destination a23-44-161-156.deploy.static.akamaitechnologies.com [23.44.161.156], a class A. 

***DHCP Packet Capture***
The below image shows me releasing my IP (thus the release DHCP packet) then seeing the Discover, Offer, Request, ACK packets which completes the DORA process. The lease time offered is 24 hours. 
<img width="950" alt="image" src="https://user-images.githubusercontent.com/94156893/230271798-ac54725e-ca92-4f9c-b028-f7fd4f1d730d.png">
<img width="501" alt="image" src="https://user-images.githubusercontent.com/94156893/230271849-57a1a762-b341-454c-ae9d-731f37b05f81.png">

***Spy on your Opponents***

The below image shows the UDP stream of me launching the game Team Fortress 2. The information is encrypted but shows the action of entering the game, selecting a class, and moving towards the objective. 
<img width="960" alt="image" src="https://user-images.githubusercontent.com/94156893/230275186-e0238119-8701-4ca7-8294-f58cd17acc61.png">
<img width="960" alt="image" src="https://user-images.githubusercontent.com/94156893/230275346-4a93b0ea-5733-41c3-bad0-cec5c57912a7.png">

***Insecure web Server***

THe below image shows the email and password I used to try and login, along with all of the web traffic that visiting this site and logging in generated. 
<img width="960" alt="image" src="https://user-images.githubusercontent.com/94156893/230275857-a994c006-6d22-4dce-a706-7da26a86c01f.png">
<img width="960" alt="image" src="https://user-images.githubusercontent.com/94156893/230275904-7a44db63-81fb-4b57-b566-79ae2aa0fdd9.png">

