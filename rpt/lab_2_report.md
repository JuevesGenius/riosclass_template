# 1. C model for original GreenRio frontend



# 2. GreenRio pipeline performance improvement: frontend



# 3. Open EDA flow
3.0 GreenRio core RTL synthesis using configuration file `config.tcl`:
![截屏2022-12-17 16 11 57](https://user-images.githubusercontent.com/115879790/208232539-fd248643-9f7a-45b3-816d-5791e9f6f122.png)

3.1 Synthesis procedure:
<img width="1027" alt="截屏2022-12-17 21 20 37" src="https://user-images.githubusercontent.com/115879790/208243907-c9cd1ab6-39aa-42ae-aedb-ba60d8e16c76.png">

3.2 The log of synthesis: `riosclass_template/openlane/RUN_2022.12.17_10.51.59/logs/synthesis`
![截屏2022-12-17 22 49 13](https://user-images.githubusercontent.com/115879790/208247645-dfd282ef-7b92-40f4-9867-241fd038ec59.png)


3.3 The result of floorplanning: `riosclass_template/openlane/RUN_2022.12.17_10.51.59/logs/floorplan`
![截屏2022-12-17 22 49 59](https://user-images.githubusercontent.com/115879790/208247675-790af464-9fdf-4132-854d-7fb699057702.png)


3.4 The result of placement: `riosclass_template/openlane/RUN_2022.12.17_10.51.59/logs/placement`
![截屏2022-12-17 22 51 12](https://user-images.githubusercontent.com/115879790/208247732-f220caa8-0d72-4a0a-be4b-1963d242840e.png)


3.5 The result of CTS: `riosclass_template/openlane/RUN_2022.12.17_10.51.59/logs/cts`
![截屏2022-12-17 22 51 39](https://user-images.githubusercontent.com/115879790/208247756-f4ea65a0-046c-4e3a-9be8-2abfd8faec32.png)


3.6 The result of global routing: `riosclass_template/openlane/RUN_2022.12.17_10.51.59/logs/routing`
![截屏2022-12-17 22 52 07](https://user-images.githubusercontent.com/115879790/208247767-87b50e52-22fd-49d1-8912-081797d5aaa3.png)
