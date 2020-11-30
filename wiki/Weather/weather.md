# ��������� ������� ������
� ��������� ����� ������� �������� �������� �������� � ������� ������ �� ���� ����������: ��������� ������� **Yandex** � ��������� ������� **OpenServiceMap**.
� ��� �������, ��� �� ������� ������������� ������������ ������ � �������� **Yandex**, ����� ��������� ��������� ������� ������ � **OpenServiceMap**.  

������� � ����� **a_def_hard.h** ���� � ������ ����������� ��� ����������, � ��� ������ ����������� - ������������ �� ������� ������ ������:  
```
#define USE_WEATHER 1         // 1 - ������������ ��������� ���������� � ������� ������; 0 - �� ������������ 
```
���� ������������� ������� ������ ��������, �������� ����� ����� ����������� �������� ������ � � Yandex � � OpenWeatherMap.   
����� ������ ������ ������ ������������ � ������ ������ ������������ ����������� � ��������� ���������� �� ���������.

## ��������� ������ � Yandex

��������� �� ���� [Yandex](http://yandex.com/), ������� ������ "�����"  

![Yandex](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/001.png)

� �������� ������ �������� ������� ����� URL � ����� ������ ������.  
���� ����� �� ��������� � �� ������ ���������, ��� ������ ���� ������������ - � ����� ������ �������� �������� � ������ � ������� Yandex �� ���������.  
���������� ��������� ��������� ������ � **OpenWeatherMap**.  

![Yandex](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/002.png)

��������� ��������� ���. ����� �������� �������� � ���������������, ������������ � ���������� �� ��������� �
�������� ���� ��� � ���� "��� �������" �� �������� �������� ��������.  

![Yandex](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/003.png)

## ��������� ������ � OpenWeatherMap

��������� �� ���� [OpenWeatherMap](http://openweathermap.org/)  
����� �� ������ ������ � ������ "Search" ������� ������ �� ���������� ��������� � ������� �� ����  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/004.png)

� �������� ������ �������� ������� ����� URL � ����� ������ ������  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/005.png)

��������� ��������� ���. ����� �������� �������� � ���������������, ������������ � ���������� �� ��������� �
�������� ���� ��� � ���� "��� �������" �� �������� �������� ��������.  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/006.png)

��������� � �������� �����, ��� ���������� ����������� � �������� � �������� ����������� ������ � ������� ������.  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/007.png)

���� ������ ��������� �� �������� ��������� ������ ������ �� ������ ������ (������ � ����� 401) �/��� ��������� � �������� ����� API, ��������� ��������� ��������:  

- ��������� �� [������](https://home.openweathermap.org/users/sign_in) � ������� � ���� ������� ������ �� c������ OpenWeatgerMap ���
�������� ��, ���� � ��� ��� ��� ������� ������.  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/008.png)

- ��������� �����, ������ � ����� ���� �����, ������, �������� ����������� email, ����������� � ��������� � ������� ������ "Create Account"  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/009.png)

- ��������� � ���� �������� ���� - ��� ������ ������ � �������� ����������� ����������� �� ������� OpenServiceMap  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/010.png)

- ������� �� ������ "Verify your email". ��� �� ����� ������ ��������� ������, � ������� ������ ��������� ��� ��� ���� API  

![OpenWeatherMap](https://github.com/vvip-68/GyverPanelWiFi/blob/master/wiki/Weather/011.png)

- � ����� a_def_soft.h � ������ 406 ������� ���������:
```
// API-������������� ������� ��������� ������                                                  
#define WEATHER_API_KEY "6a4ba421859c9f4166697758b68d889b"
```
� �������� ���� �� ���������� ���� � �������� ������. ��� �������, ���� ������������ � ������� 10 �����, ���� - �� ���� �����.  
��������� ��������� �����, ����� ������� �� ������ ������� ��������� � API �� ������ � �������� ����� ���������� �� ������, �
JSON � ����������� � ������� ������.  
```
{"coord":{"lon":92.79,"lat":56.01},"weather":[{"id":803,"main":"Clouds","description":"broken clouds","icon":"04d"}],"base":"stations",  
"main":{"temp":-1,"feels_like":-6.3,"temp_min":-1,"temp_max":-1,"pressure":1023,"humidity":80},"visibility":10000,"wind":{"speed":4,"deg":270},  
"clouds":{"all":75},"dt":1604373691,"sys":{"type":1,"id":8957,"country":"RU","sunrise":1604365212,"sunset":1604397872},  
"timezone":25200,"id":1502026,"name":"Krasnoyarsk","cod":200}
```
��������� �������� � ����� ������ � ����������. ��������� � �������� �����, ��� � ����� ���� ���������� �� �������� �������� ������ � ��������� �������.

