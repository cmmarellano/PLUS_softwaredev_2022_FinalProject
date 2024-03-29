
*Practice: Software Development - 22S* <br>
*Final Project*

## “Open Routing in Python”: Building a Routing application using Folium, Geopy, and Open Routes Service API 

![image](https://user-images.githubusercontent.com/93019319/172910297-64dc0d28-7c0a-4cc4-9103-f7c8c5529745.png)
*Sample routing in Folium [Towards DataScience, 2020](https://towardsdatascience.com/build-interactive-gps-activity-maps-from-gpx-files-using-folium-cf9eebba1fe7)*

### Project Summary
<br>

*Motivation*
- To explore the use of different geo python libraries that provides simple services such as geocoding, route-finding, and map visualization

We propose a python application that allows geocoding from street addresses of location dataset. These geocoded locations will be mapped and be the basis for the main functionality of this project application - routing.

The routing functionality will perform route-finding from a user location derived from user IP address to a user defined location (selected from dropdown list of the geocoded addresses). The actual shortest route path(drive path) will then be visualized on the map, and presented along with the measured distance (by car). 
<br>

##### Team Members
Arellano, Carla Mae  [@cmmarellano](https://www.github.com/cmmarellano) <br>
Adriko, Kennedy  [@adken](https://www.github.com/adken)
<br>
<br>

### Methodology

<br>

Data Required:
- Administrative Addresses 
<br>

Study / Test Area:
- Austria
- EU
<br>

Python libraries:
- Geopy
- Folium
- Open Routes Service API
- Pandas
- Leafmap
- Nominatim
- Etc. (as needed)
<br>

Steps taken:
- Implement geocoding
- Plot geocoded locations on web map
- Implement routing from user selected origin to user selected destination on the map
- Visualize optimal driving route
- Calculate distance for optimal driving route
<br>

-------


### Results :

@28.08.2022 <br>

*See final notebook for implementation [Map_routing.ipynb](https://github.com/cmmarellano/PLUS_softwaredev_2022_FinalProject/blob/main/Map_routing.ipynb)
<br>

![](https://github.com/cmmarellano/PLUS_softwaredev_2022_FinalProject/blob/main/img/Sample_gif.gif)

_Destination selection, route computation from user location, and mappping_


<br>

----


### Project Timeline

Project Deadline: ***July 10, 2022 / August 2022***

<br>
- Timeline of Activities

![image](https://user-images.githubusercontent.com/93019319/172907631-37a2f179-92d7-4886-b53b-04a8d9b4e0cc.png)

<br>
Responsibilities:
<br>

- Carla (at least 15 hrs)
  - Geocoding
  - Mapping + Interface
  - Testing
  - Improvements
<br>

- Kennedy (at least 15 hrs)
  - Geocoding
  - Routing
  - Testing
  - Improvements


----

### General Instructions

Update:
@ 28.08.2022.

1. Create the environment '[sde_project](https://github.com/cmmarellano/PLUS_softwaredev_2022_FinalProject/blob/main/sde_project_env.yml)'
  - Libraries installed
    - folium
    - geopy
    - openrouteservice
    - pandas


```
(sde_project) C:\Users\carellano.LEGION5PRO-O3OB\.conda\envs\sde_project>conda list
# packages in environment at C:\Users\carellano.LEGION5PRO-O3OB\.conda\envs\sde_project:
#
# Name                    Version                   Build  Channel
altair                    4.2.0              pyhd8ed1ab_1    conda-forge
anyio                     3.6.1            py39hcbf5309_0    conda-forge
appdirs                   1.4.4                    pypi_0    pypi
argon2-cffi               21.3.0             pyhd8ed1ab_0    conda-forge
argon2-cffi-bindings      21.2.0           py39hb82d6ee_2    conda-forge
arrow-cpp                 8.0.0            py39hbd6f097_0
asttokens                 2.0.5              pyhd8ed1ab_0    conda-forge
attrs                     21.4.0             pyhd8ed1ab_0    conda-forge
aws-c-common              0.4.57               ha925a31_1
aws-c-event-stream        0.1.6                hd77b12b_5
aws-checksums             0.1.9                ha925a31_0
aws-sdk-cpp               1.8.185              hd77b12b_0
babel                     2.10.3             pyhd8ed1ab_0    conda-forge
backcall                  0.2.0              pyh9f0ad1d_0    conda-forge
backports                 1.0                        py_2    anaconda
backports.functools_lru_cache 1.6.4              pyhd8ed1ab_0    conda-forge
beautifulsoup4            4.11.1             pyha770c72_0    conda-forge
bleach                    5.0.0              pyhd8ed1ab_0    conda-forge
blinker                   1.4                        py_1    conda-forge
boost-cpp                 1.80.0               h9f4b32c_0    conda-forge
bqplot                    0.12.33            pyhd8ed1ab_0    conda-forge
branca                    0.5.0              pyhd8ed1ab_0    conda-forge
brotli                    1.0.9                h8ffe710_7    conda-forge
brotli-bin                1.0.9                h8ffe710_7    conda-forge
brotlipy                  0.7.0           py39hb82d6ee_1004    conda-forge
bzip2                     1.0.8                h8ffe710_4    conda-forge
c-ares                    1.18.1               h8ffe710_0    conda-forge
ca-certificates           2022.6.15            h5b45459_0    conda-forge
cachetools                5.2.0              pyhd8ed1ab_0    conda-forge
certifi                   2022.6.15          pyhd8ed1ab_1    conda-forge
cffi                      1.15.0           py39h0878f49_0    conda-forge
charset-normalizer        2.0.12             pyhd8ed1ab_0    conda-forge
click                     8.1.3            py39hcbf5309_0    conda-forge
colorama                  0.4.5              pyhd8ed1ab_0    conda-forge
colour                    0.1.5                      py_0    conda-forge
commonmark                0.9.1                      py_0    conda-forge
cryptography              37.0.2           py39h7bc7c5c_0    conda-forge
cycler                    0.11.0             pyhd8ed1ab_0    conda-forge
dataclasses               0.8                pyhc8e2a94_3    conda-forge
debugpy                   1.6.0            py39h415ef7b_0    conda-forge
decorator                 5.1.1              pyhd8ed1ab_0    conda-forge
defusedxml                0.7.1              pyhd8ed1ab_0    conda-forge
entrypoints               0.4                pyhd8ed1ab_0    conda-forge
executing                 0.8.3              pyhd8ed1ab_0    conda-forge
filelock                  3.7.1              pyhd8ed1ab_0    conda-forge
flask                     2.2.2                    pypi_0    pypi
flit-core                 3.7.1              pyhd8ed1ab_0    conda-forge
folium                    0.12.1.post1       pyhd8ed1ab_1    conda-forge
fonttools                 4.33.3           py39hb82d6ee_0    conda-forge
freetype                  2.10.4               h546665d_1    conda-forge
future                    0.18.2           py39hcbf5309_5    conda-forge
gdown                     4.4.0              pyhd8ed1ab_0    conda-forge
geographiclib             1.52               pyhd8ed1ab_0    conda-forge
geojson                   2.5.0                      py_0    conda-forge
geopy                     2.2.0              pyhd8ed1ab_0    conda-forge
gflags                    2.2.2             ha925a31_1004    conda-forge
gitdb                     4.0.9              pyhd8ed1ab_0    conda-forge
gitpython                 3.1.27             pyhd8ed1ab_0    conda-forge
glog                      0.6.0                h4797de2_0    conda-forge
idna                      3.3                pyhd8ed1ab_0    conda-forge
importlib-metadata        4.11.4           py39hcbf5309_0    conda-forge
importlib_metadata        4.11.4               hd8ed1ab_0    conda-forge
importlib_resources       5.8.0              pyhd8ed1ab_0    conda-forge
intel-openmp              2022.1.0          h57928b3_3787    conda-forge
ipyevents                 2.0.1              pyhd8ed1ab_0    conda-forge
ipyfilechooser            0.6.0              pyhd8ed1ab_0    conda-forge
ipykernel                 6.14.0           py39h832f523_0    conda-forge
ipyleaflet                0.16.0             pyhd8ed1ab_4    conda-forge
ipysheet                  0.5.0              pyhd8ed1ab_0    conda-forge
ipython                   8.4.0            py39hcbf5309_0    conda-forge
ipython_genutils          0.2.0                      py_1    conda-forge
ipytree                   0.2.1              pyhd8ed1ab_0    conda-forge
ipywidgets                7.7.0              pyhd8ed1ab_0    conda-forge
itsdangerous              2.1.2                    pypi_0    pypi
jedi                      0.18.1           py39hcbf5309_1    conda-forge
jinja2                    3.1.2              pyhd8ed1ab_1    conda-forge
joblib                    1.1.0              pyhd8ed1ab_0    conda-forge
jpeg                      9e                   h8ffe710_1    conda-forge
json5                     0.9.5              pyh9f0ad1d_0    conda-forge
jsonschema                4.6.0              pyhd8ed1ab_0    conda-forge
jupyter_client            7.3.4              pyhd8ed1ab_0    conda-forge
jupyter_core              4.10.0           py39hcbf5309_0    conda-forge
jupyter_server            1.17.1             pyhd8ed1ab_0    conda-forge
jupyterlab                3.4.3              pyhd8ed1ab_0    conda-forge
jupyterlab_pygments       0.2.2              pyhd8ed1ab_0    conda-forge
jupyterlab_server         2.14.0             pyhd8ed1ab_0    conda-forge
jupyterlab_widgets        1.1.0              pyhd8ed1ab_0    conda-forge
kiwisolver                1.4.3            py39h2e07f2f_0    conda-forge
krb5                      1.19.3               h1176d77_0    conda-forge
lcms2                     2.12                 h2a16943_0    conda-forge
leafmap                   0.9.4              pyhd8ed1ab_0    conda-forge
lerc                      3.0                  h0e60522_0    conda-forge
libblas                   3.9.0              15_win64_mkl    conda-forge
libbrotlicommon           1.0.9                h8ffe710_7    conda-forge
libbrotlidec              1.0.9                h8ffe710_7    conda-forge
libbrotlienc              1.0.9                h8ffe710_7    conda-forge
libcblas                  3.9.0              15_win64_mkl    conda-forge
libcurl                   7.83.1               h789b8ee_0    conda-forge
libdeflate                1.12                 h8ffe710_0    conda-forge
liblapack                 3.9.0              15_win64_mkl    conda-forge
libpng                    1.6.37               h1d00b33_2    conda-forge
libprotobuf               3.20.1               h7755175_1    conda-forge
libsodium                 1.0.18               h8d14728_1    conda-forge
libssh2                   1.10.0               h680486a_3    conda-forge
libthrift                 0.15.0               h636ae23_1    conda-forge
libtiff                   4.4.0                h2ed3b44_1    conda-forge
libwebp                   1.2.2                h57928b3_0    conda-forge
libwebp-base              1.2.2                h8ffe710_1    conda-forge
libxcb                    1.13              hcd874cb_1004    conda-forge
libzlib                   1.2.12               h8ffe710_1    conda-forge
lz4-c                     1.9.3                h8ffe710_1    conda-forge
m2w64-gcc-libgfortran     5.3.0                         6    conda-forge
m2w64-gcc-libs            5.3.0                         7    conda-forge
m2w64-gcc-libs-core       5.3.0                         7    conda-forge
m2w64-gmp                 6.1.0                         2    conda-forge
m2w64-libwinpthread-git   5.0.0.4634.697f757               2    conda-forge
mapclassify               2.4.3              pyhd8ed1ab_0    conda-forge
markupsafe                2.1.1            py39hb82d6ee_1    conda-forge
matplotlib-base           3.5.2            py39h581301d_0    conda-forge
matplotlib-inline         0.1.3              pyhd8ed1ab_0    conda-forge
mistune                   0.8.4           py39hb82d6ee_1005    conda-forge
mkl                       2022.1.0           h6a75c08_874    conda-forge
msys2-conda-epoch         20160418                      1    conda-forge
munkres                   1.1.4              pyh9f0ad1d_0    conda-forge
nbclassic                 0.3.7              pyhd8ed1ab_0    conda-forge
nbclient                  0.6.4              pyhd8ed1ab_1    conda-forge
nbconvert                 6.5.0              pyhd8ed1ab_0    conda-forge
nbconvert-core            6.5.0              pyhd8ed1ab_0    conda-forge
nbconvert-pandoc          6.5.0              pyhd8ed1ab_0    conda-forge
nbformat                  5.4.0              pyhd8ed1ab_0    conda-forge
nest-asyncio              1.5.5              pyhd8ed1ab_0    conda-forge
networkx                  2.8.4              pyhd8ed1ab_0    conda-forge
notebook                  6.4.12             pyha770c72_0    conda-forge
notebook-as-pdf           0.5.0                    pypi_0    pypi
notebook-shim             0.1.0              pyhd8ed1ab_0    conda-forge
numpy                     1.22.4           py39h0948cea_0    conda-forge
openjpeg                  2.4.0                hb211442_1    conda-forge
openrouteservice          2.3.3                    pypi_0    pypi
openssl                   1.1.1q               h8ffe710_0    conda-forge
packaging                 21.3               pyhd8ed1ab_0    conda-forge
pandas                    1.4.2            py39h2e25243_2    conda-forge
pandoc                    2.2                      pypi_0    pypi
pandocfilters             1.5.0              pyhd8ed1ab_0    conda-forge
parso                     0.8.3              pyhd8ed1ab_0    conda-forge
pickleshare               0.7.5                   py_1003    conda-forge
pillow                    9.1.1            py39ha53f419_1    conda-forge
pip                       21.2.4           py39haa95532_0    anaconda
plumbum                   1.7.2                    pypi_0    pypi
ply                       3.11                     pypi_0    pypi
prometheus_client         0.14.1             pyhd8ed1ab_0    conda-forge
prompt-toolkit            3.0.29             pyha770c72_0    conda-forge
protobuf                  3.20.1           py39hcbf5309_0    conda-forge
pscript                   0.7.5              pyhd3deb0d_0    conda-forge
psutil                    5.9.1            py39hb82d6ee_0    conda-forge
pthread-stubs             0.4               hcd874cb_1001    conda-forge
pure_eval                 0.2.2              pyhd8ed1ab_0    conda-forge
pyarrow                   9.0.0                    pypi_0    pypi
pycparser                 2.21               pyhd8ed1ab_0    conda-forge
pycrs                     1.0.2                      py_0    conda-forge
pydeck                    0.7.1              pyh6c4a22f_0    conda-forge
pyee                      8.2.2                    pypi_0    pypi
pygments                  2.12.0             pyhd8ed1ab_0    conda-forge
pympler                   1.0.1              pyhd8ed1ab_0    conda-forge
pyopenssl                 22.0.0             pyhd8ed1ab_0    conda-forge
pyparsing                 3.0.9              pyhd8ed1ab_0    conda-forge
pypdf2                    2.10.3                   pypi_0    pypi
pyppeteer                 1.0.2                    pypi_0    pypi
pyrsistent                0.18.1           py39hb82d6ee_1    conda-forge
pyshp                     2.3.0              pyhd8ed1ab_0    conda-forge
pysocks                   1.7.1            py39hcbf5309_5    conda-forge
pystac                    1.4.0              pyhd8ed1ab_0    conda-forge
pystac-client             0.4.0              pyhd8ed1ab_0    conda-forge
python                    3.9.7                h6244533_1    anaconda
python-box                6.0.2              pyhd8ed1ab_0    conda-forge
python-dateutil           2.8.2              pyhd8ed1ab_0    conda-forge
python-fastjsonschema     2.15.3             pyhd8ed1ab_0    conda-forge
python-tzdata             2022.2             pyhd8ed1ab_0    conda-forge
python_abi                3.9                      2_cp39    conda-forge
pytz                      2022.1             pyhd8ed1ab_0    conda-forge
pytz-deprecation-shim     0.1.0.post0      py39hcbf5309_2    conda-forge
pywin32                   303              py39hb82d6ee_0    conda-forge
pywinpty                  2.0.2            py39h5da7b33_0    anaconda
pyyaml                    6.0              py39hb82d6ee_4    conda-forge
pyzmq                     23.1.0           py39he46f08e_0    conda-forge
re2                       2022.04.01           h0e60522_0    conda-forge
requests                  2.28.0             pyhd8ed1ab_0    conda-forge
rich                      12.5.1             pyhd8ed1ab_0    conda-forge
ruamel.yaml               0.17.21          py39hb82d6ee_1    conda-forge
ruamel.yaml.clib          0.2.6            py39hb82d6ee_1    conda-forge
scikit-learn              1.1.1            py39he931e04_0    conda-forge
scipy                     1.8.1            py39hc0c34ad_0    conda-forge
semver                    2.13.0             pyh9f0ad1d_0    conda-forge
send2trash                1.8.0              pyhd8ed1ab_0    conda-forge
setuptools                61.2.0           py39haa95532_0    anaconda
six                       1.16.0             pyh6c4a22f_0    conda-forge
smmap                     3.0.5              pyh44b312d_0    conda-forge
snappy                    1.1.9                h82413e6_1    conda-forge
sniffio                   1.2.0            py39hcbf5309_3    conda-forge
soupsieve                 2.3.1              pyhd8ed1ab_0    conda-forge
sqlite                    3.38.3               h2bbff1b_0    anaconda
stack_data                0.3.0              pyhd8ed1ab_0    conda-forge
streamlit                 1.12.0                   pypi_0    pypi
streamlit-folium          0.6.14                   pypi_0    pypi
tbb                       2021.5.0             h2d74725_1    conda-forge
terminado                 0.15.0           py39hcbf5309_0    conda-forge
threadpoolctl             3.1.0              pyh8a188c0_0    conda-forge
tinycss2                  1.1.1              pyhd8ed1ab_0    conda-forge
tk                        8.6.12               h8ffe710_0    conda-forge
toml                      0.10.2             pyhd8ed1ab_0    conda-forge
toolz                     0.12.0             pyhd8ed1ab_0    conda-forge
tornado                   6.1              py39hb82d6ee_3    conda-forge
tqdm                      4.64.0             pyhd8ed1ab_0    conda-forge
traitlets                 5.3.0              pyhd8ed1ab_0    conda-forge
traittypes                0.2.1              pyh9f0ad1d_2    conda-forge
typing_extensions         4.3.0              pyha770c72_0    conda-forge
tzdata                    2022a                hda174b7_0    anaconda
tzlocal                   4.2              py39hcbf5309_1    conda-forge
unicodedata2              14.0.0           py39hb82d6ee_1    conda-forge
urllib3                   1.26.9             pyhd8ed1ab_0    conda-forge
utf8proc                  2.6.1                h2bbff1b_0
validators                0.18.2             pyhd3deb0d_0    conda-forge
vc                        14.2                 h21ff451_1    anaconda
vs2015_runtime            14.27.29016          h5e58377_2    anaconda
watchdog                  2.1.9            py39hcbf5309_0    conda-forge
wcwidth                   0.2.5              pyh9f0ad1d_2    conda-forge
webencodings              0.5.1                      py_1    conda-forge
websocket-client          1.3.2              pyhd8ed1ab_0    conda-forge
websockets                10.3                     pypi_0    pypi
wheel                     0.37.1             pyhd3eb1b0_0    anaconda
whitebox                  2.1.2              pyhd8ed1ab_0    conda-forge
whiteboxgui               0.7.0              pyhd8ed1ab_0    conda-forge
widgetsnbextension        3.6.0            py39hcbf5309_0    conda-forge
win_inet_pton             1.1.0            py39hcbf5309_4    conda-forge
wincertstore              0.2              py39haa95532_2    anaconda
winpty                    0.4.3                         4    anaconda
xorg-kbproto              1.0.7             hcd874cb_1002    conda-forge
xorg-libx11               1.7.2                hcd874cb_0    conda-forge
xorg-libxau               1.0.9                hcd874cb_0    conda-forge
xorg-libxdmcp             1.1.3                hcd874cb_0    conda-forge
xorg-xproto               7.0.31            hcd874cb_1007    conda-forge
xyzservices               2022.4.0           pyhd8ed1ab_0    conda-forge
xz                        5.2.5                h62dcd97_1    conda-forge
yaml                      0.2.5                h8ffe710_2    conda-forge
zeromq                    4.3.4                h0e60522_1    conda-forge
zipp                      3.8.0              pyhd8ed1ab_0    conda-forge
zlib                      1.2.12               h8ffe710_1    conda-forge
zstd                      1.5.2                h6255e5f_1    conda-forge

```

2. Obtain Openrouteservice API key
3. Run the notebook: [Map_routing.ipynb](https://github.com/cmmarellano/PLUS_softwaredev_2022_FinalProject/blob/main/Map_routing.ipynb)
4. Append key on OSR client
5. On file upload widget, input [restaurants.csv](https://github.com/cmmarellano/PLUS_softwaredev_2022_FinalProject/blob/main/restaurant.csv)
6. Run geocoding
7. On dropdown widget, select a 'destination'
8. Run mapping code to obtain the map visualization and route information! ;)



----


### References
-	https://towardsdatascience.com/visualization-in-python-finding-routes-between-points-2d97d4881996
-	https://python.plainenglish.io/exploring-open-route-service-api-820a0ccffecc
-	https://github.com/GIScience/openrouteservice
-	https://giswqs.medium.com/a-jupyter-notebook-example-for-interactive-mapping-with-earth-engine-ipyleaflet-and-ipywidgets-f1790a9fae0d
-	https://openrouteservice-py.readthedocs.io/en/latest/
-	https://towardsdatascience.com/build-interactive-gps-activity-maps-from-gpx-files-using-folium-cf9eebba1fe7
-	https://discuss.streamlit.io/t/ann-streamlit-folium-a-component-for-rendering-folium-maps/4367
-	https://ask.openrouteservice.org/t/getting-a-distance/1513

