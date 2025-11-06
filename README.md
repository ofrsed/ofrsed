rypi:~ $ ls /dev/input/
by-id    event0  event10  event3  event5  event7  event9  mouse0  mouse2
by-path  event1  event2   event4  event6  event8  mice    mouse1
root1@raspberrypi:~ $ cat /proc/bus/input/devices 
I: Bus=0003 Vendor=5566 Product=0008 Version=0110
N: Name="RGBMicroChip PANTEON T2 PRO RS Keyboard"
P: Phys=usb-0000:01:00.0-1.2/input0
S: Sysfs=/devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input0
U: Uniq=2022-12-12
H: Handlers=kbd leds event0 
B: PROP=0
B: EV=12001f
B: KEY=33eff 0 0 483ffff17aff32d bfd4444600000000 1 130c730b17c007 ffa67bfad941dfff 80beffcd01cfffff febffbffdffffffe
B: REL=1040
B: ABS=100000000
B: MSC=10
B: LED=1f

I: Bus=0003 Vendor=5566 Product=0008 Version=0110
N: Name="RGBMicroChip PANTEON T2 PRO RS Mouse"
P: Phys=usb-0000:01:00.0-1.2/input0
S: Sysfs=/devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input2
U: Uniq=2022-12-12
H: Handlers=mouse0 event1 
B: PROP=0
B: EV=17
B: KEY=1f0000 0 0 0 0
B: REL=1943
B: MSC=10

I: Bus=0003 Vendor=5566 Product=0008 Version=0110
N: Name="RGBMicroChip PANTEON T2 PRO RS Wireless Radio Control"
P: Phys=usb-0000:01:00.0-1.2/input0
S: Sysfs=/devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input3
U: Uniq=2022-12-12
H: Handlers=event2 
B: PROP=0
B: EV=13
B: KEY=1 0 0 0 0
B: MSC=10

I: Bus=0003 Vendor=5566 Product=0008 Version=0110
N: Name="RGBMicroChip PANTEON T2 PRO RS"
P: Phys=usb-0000:01:00.0-1.2/input1
S: Sysfs=/devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.1/0003:5566:0008.0002/input/input4
U: Uniq=2022-12-12
H: Handlers=sysrq kbd leds event3 
B: PROP=0
B: EV=120013
B: KEY=1000000000007 ff9f207ac14057ff febeffdfffefffff fffffffffffffffe
B: MSC=10
B: LED=1f

I: Bus=0003 Vendor=5566 Product=0008 Version=0110
N: Name="RGBMicroChip PANTEON T2 PRO RS"
P: Phys=usb-0000:01:00.0-1.2/input2
S: Sysfs=/devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.2/0003:5566:0008.0003/input/input5
U: Uniq=2022-12-12
H: Handlers=event4 
B: PROP=0
B: EV=9
B: ABS=10000000000

I: Bus=001e Vendor=0000 Product=0000 Version=0001
N: Name="vc4-hdmi-0"
P: Phys=vc4-hdmi-0/input0
S: Sysfs=/devices/platform/soc/fef00700.hdmi/rc/rc0/input6
U: Uniq=
H: Handlers=kbd event5 
B: PROP=20
B: EV=100017
B: KEY=ffffc000000000 3ff 0 400000320fc200 40830c900000000 0 210300 49d2c040ec00 1e378000000000 8010000010000000
B: REL=3
B: MSC=10

I: Bus=0000 Vendor=0000 Product=0000 Version=0000
N: Name="vc4-hdmi-0 HDMI Jack"
P: Phys=ALSA
S: Sysfs=/devices/platform/soc/fef00700.hdmi/sound/card1/input7
U: Uniq=
H: Handlers=event6 
B: PROP=0
B: EV=21
B: SW=40

I: Bus=001e Vendor=0000 Product=0000 Version=0001
N: Name="vc4-hdmi-1"
P: Phys=vc4-hdmi-1/input0
S: Sysfs=/devices/platform/soc/fef05700.hdmi/rc/rc1/input8
U: Uniq=
H: Handlers=kbd event7 
B: PROP=20
B: EV=100017
B: KEY=ffffc000000000 3ff 0 400000320fc200 40830c900000000 0 210300 49d2c040ec00 1e378000000000 8010000010000000
B: REL=3
B: MSC=10

I: Bus=0000 Vendor=0000 Product=0000 Version=0000
N: Name="vc4-hdmi-1 HDMI Jack"
P: Phys=ALSA
S: Sysfs=/devices/platform/soc/fef05700.hdmi/sound/card2/input9
U: Uniq=
H: Handlers=event8 
B: PROP=0
B: EV=21
B: SW=40

I: Bus=001c Vendor=0000 Product=1ea6 Version=0000
N: Name="ADS7846 Touchscreen"
P: Phys=spi0.0/input0
S: Sysfs=/devices/platform/soc/fe204000.spi/spi_master/spi0/spi0.0/input/input10
U: Uniq=
H: Handlers=mouse1 event9 
B: PROP=0
B: EV=b
B: KEY=400 0 0 0 0 0
B: ABS=1000003

I: Bus=0005 Vendor=046d Product=b015 Version=0013
N: Name="Logitech M720 Triathlon Multi-Device Mouse"
P: Phys=2c:cf:67:f3:4c:06
S: Sysfs=/devices/virtual/misc/uhid/0005:046D:B015.0004/input/input14
U: Uniq=c9:d8:7c:c0:7b:e3
H: Handlers=sysrq kbd mouse2 event10 
B: PROP=0
B: EV=100017
B: KEY=ffff0000 1000000000007 ff800000000007ff febeffdfffefffff fffffffffffffffe
B: REL=1943
B: MSC=10



## Hi there 👋
<div id="header" align="center">
  <img src="https://github.com/ofrsed/ofrsed/blob/main/bongo-cat-typing.gif" width="100"/>
</div>


<div id="badges" align="center">
  <a href="https://t.me/ofrsed">
    <img src="https://img.shields.io/badge/Telegram-blue?style=for-the-badge&logo=telegram&logoColor=white" alt="LinkedIn Badge"/>
 
  </a>
</div>

## Intro

I started getting interested in programming while still working as an automation engineer. My acquaintance began with Arduino (C++), but then I got interested in Python. After some time, the company closed, and I decided to delve even deeper into IT. And this is, of course, complete madness 🧐. I spent almost a year looking for a job, surviving on Telegram bots, small sites and parsing :anguished: (Press F). Now I am putting my efforts into a cool company.

## Language and Tools
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" title="python" alt="python" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/pytest/pytest-original.svg" title="pytest" alt="pytest" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" title="php" alt="php" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/lua/lua-original.svg" title="lua" alt="lua" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/django/django-plain.svg" title="django" alt="django" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/postman/postman-original.svg" title="postman" alt="postman" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/djangorest/djangorest-original.svg" title="djangorest" alt="djangorest" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/flask/flask-original.svg" title="flask" alt="flask" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg"  title="CSS3" alt="CSS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="MySQL"  alt="MySQL" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/git/git-original-wordmark.svg" title="Git" **alt="Git" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/gitlab/gitlab-original.svg" title="gitlab" **alt="gitlab" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/figma/figma-original.svg" title="figma" **alt="figma" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/pycharm/pycharm-original.svg" title="pycharm" **alt="pycharm" width="40" height="40"/>
</div>


## Certificates
<div>
<h1>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/1-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/2-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/3-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/4-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/5-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/6-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/7-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/8-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/9-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/10-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/11-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/12-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/13-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/14-1.png" width="200px"/>


</h1>
</div>

## Notes / Road map

Programming language
  - [x] [Python](https://github.com/ofrsed/Notes/blob/main/Python/python_notes.md)
    - [x] [OOP](https://github.com/ofrsed/Notes/blob/main/Python/python_oop_notes.md)
    - [x] Frameworks
      - [x] [Asyncio](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/asyncio.md), [Multithreading](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/multithreading.md),  [Matplotlib](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/matplotlib.md), Aiogram, BeautifulSoup4, Selenium, Django, Flask
      - [ ] Pandas, NumPy
  - [ ] [C++](https://github.com/ofrsed/Notes/blob/main/%D0%A1/C%2B%2B.md)
  - [ ] [JS](https://github.com/ofrsed/Notes/blob/main/JavaScript/javascript_notes.md)
  - [x] PHP

- Databases and SQL
  - [x] [Neo4j](https://github.com/ofrsed/Notes/blob/main/neo4j/neo4j_notes.md)
  - [x] [SQL](https://github.com/ofrsed/Notes/blob/main/SQL/sql_notes.md)
  - [x] Redis
- Data structures and algorithms
  - [x] [Структуры данных](https://github.com/ofrsed/Notes/blob/main/data%20structures%20and%20algorithms/data%20structures.md) 
  - [x] [Grokking Algorithms](https://github.com/ofrsed/ofrsed/blob/main/Grokaem_algoritmy.pdf)
- VCS
  - [x] Git
- Communication as a Service
  - [x] [k8s](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/k8s.md)
  - [x] [Docker](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/docker.md)
  - [x] [Брокеры сообщений](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/message_broker.md)
- Operating System
  - [x] [Linux](https://github.com/ofrsed/Notes/blob/main/Linux/linux_notes.md)
  - [x] Windows 


## Tasks

- [ ] [🎥](https://www.youtube.com/watch?v=WlCDcr8JYFU) __Clean Architecture__ 5:57 6:03-7:10

<details>
  <summary>Запланированные задачи</summary>

- [ ] 📚 __Поколение Python: алгоритмы и структуры данных__ - курс выходит 1 апреля  
- [ ] [📚](https://stepik.org/course/193691/syllabus) __C/C++__
- [ ] [🎥](https://www.youtube.com/watch?v=eDuuKvIWzew&list=PLA0M1Bcd0w8zmegfAUfFMiACPKfdW4ifD) __NumPy__
- [ ] [🎥](https://www.youtube.com/watch?v=HemPVRvVm40&list=PLBP4Q3FNSLK2EujXiPUeTIOVnydZS8YJk) __Pandas__
- [ ] [🎥](https://www.youtube.com/watch?v=gA3A_epB3So&t=755s) __База по оптимизации PostgreSQL__
- [ ] 🌐 __K8S__
- [ ] 🌐 __модуль OS__
- [ ] 🌐 __Chrome DevTools__
- [ ] 🌐 __1C__
- [ ] 🌐 __Bitrix__
- [ ] 🌐 __Балансировщики нагрузки__
- [ ] 🌐 __sqlalchemy (доп.)__
- [ ] 🌐 __WSGI__
- [ ] 🌐 __TDD__
- [ ] 🌐 __профилирование__

sqlalchemy 
</details>
<details>
  <summary>Завершенные задачи</summary>

от 15.02
- [x] [📚](https://stepik.org/course/199114/syllabus) Брокеры сообщений. Apache Kafka
- [x] [🎥](https://www.youtube.com/watch?v=bcMZGPIeGzk) __Middleware in FastAPI__
- [x] [🎥](https://www.youtube.com/playlist?list=PLDyvV36pndZFHXjXuwA_NywNrVQO0aQqb) __GIT (пусть хранится тут)__
- [x] [🎥](https://www.youtube.com/watch?v=dKxiHlZvULQ) __Типизирование (пусть хранится тут)__

</details>

## Hot Keys

`DELETE FROM alembic_version;`

`alembic revision --autogenerate`

`alembic upgrade head`

`alembic stamp head`


## interview questions
[for interview](https://github.com/ofrsed/Notes/blob/main/interview_questions.md)

[Памятка PHP/GoLang разработчику](https://backendinterview.ru/os)

[math](https://github.com/ofrsed/Notes/blob/main/math.md)

[база #2](https://github.com/yakimka/python_interview_questions)




<!--
**ofrsed/ofrsed** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
