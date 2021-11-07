# Check-NorthKorea-DPRK-IP-Using-GeoLite
North Korea(DPRK) IP할당 대역 / 위도, 경도 확인하기
 * Ubuntu 20.04
 * Maxmind GeoLite2 data file

한국인터넷정보센터(KRNIC)의 국가별 IP 할당 대역을 보면,
![Screenshot from 2021-08-12 20-07-23](https://user-images.githubusercontent.com/47383452/129186969-57c9a619-f3a3-49e9-8454-9bd5bd3775ce.png)

Prefix /22로 1,024개의 IP대역이 할당 되어있음

Ubuntu terminal GeoLite2 데이터(AS번호, 국가, 도시명)를 열어서 확인해보겠습니다. 해당 데이터는 매주 화요일에 업데이트 되며, 해당 사이트에서 다운로드 가능합니다.

![Screenshot from 2021-08-12 20-28-49](https://user-images.githubusercontent.com/47383452/129189496-00130463-2617-4232-acfa-e6166b7e7413.png)

국가코드 "KP"로 보면, 위와 같이 geoname_id는 1873107
다시, City데이터로 보았을 때, locale_code는 다르지만 TIME ZONE은 해당칼럼이 평양으로 확인됩니다.

![Screenshot from 2021-08-12 20-43-02](https://user-images.githubusercontent.com/47383452/129191098-d1f4f686-e469-40ad-8e83-2b1c73bbe9e9.png)

Geoname_id로 IPv4 Block을 확인해보면, 아까 KRNIC에 나온 175.45.176.0/22 외 6건의 IP대역이 확인됐습니다.
Cymru로도 체크해보았는데, ASNUM을 대조해보면 다른 결과를 얻을 수 있었습니다.

![Screenshot from 2021-08-12 21-38-24](https://user-images.githubusercontent.com/47383452/129198120-5c7953df-5009-49ac-b81e-7cf77a1db767.png)

각각 북한 AS와 관련(연결)있는 AS로 유추

![Screenshot from 2021-08-12 20-46-55](https://user-images.githubusercontent.com/47383452/129191977-6efd9ced-de9f-4ae3-aa2e-c2f940dbaee3.png)
