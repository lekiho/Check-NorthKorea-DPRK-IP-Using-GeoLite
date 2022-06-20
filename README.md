# Check-NorthKorea-DPRK-IP-Using-GeoLite
North Korea(DPRK) IP
 * Maxmind GeoLite2 data file

한국인터넷정보센터(KRNIC)의 국가별 IP
![Screenshot from 2021-08-12 20-07-23](https://user-images.githubusercontent.com/47383452/129186969-57c9a619-f3a3-49e9-8454-9bd5bd3775ce.png)

Prefix /22 1,024

Ubuntu terminal GeoLite2 (AS번호, 국가, 도시명). 
![Screenshot from 2021-08-12 20-28-49](https://user-images.githubusercontent.com/47383452/129189496-00130463-2617-4232-acfa-e6166b7e7413.png)

국가코드 "KP"로 보면, 위와 같이 geoname_id는 1873107
City데이터로 보았을 때, locale_code/ TIME ZONE

![Screenshot from 2021-08-12 20-43-02](https://user-images.githubusercontent.com/47383452/129191098-d1f4f686-e469-40ad-8e83-2b1c73bbe9e9.png)

Geoname_id로 IPv4 Block을 확인해보면, 아까 KRNIC에 나온 175.45.176.0/22 외 6건의 IP대역이 확인.
Cymru로도 체크, ASNUM을 대조해보면 다른 결과를 얻을 수 있었음.

![Screenshot from 2021-08-12 21-38-24](https://user-images.githubusercontent.com/47383452/129198120-5c7953df-5009-49ac-b81e-7cf77a1db767.png)

![Screenshot from 2021-08-12 20-46-55](https://user-images.githubusercontent.com/47383452/129191977-6efd9ced-de9f-4ae3-aa2e-c2f940dbaee3.png)
