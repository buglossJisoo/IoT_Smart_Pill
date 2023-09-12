# IoT 스마트 약통
## 1. 프로젝트 주제 선정 배경

> 많은 제품들 중 약통을 메인 주제로 선정한 이유는 COVID-19로 인해 건강 유의에 대한 인식이
높아지면서 영양제의 판매량이 급증한 것에 있다. 영양제에 대한 관심과 소비가 급격히 늘어나고는
있지만 정작 규칙적으로 영양제를 전부 복용하는 사람은 많지 않아 유통기한을 지나 버리게 되는
약들이 대량 생성되어지고 있다. 이는 환경오염으로도 이어지기 때문에 약도 규칙적으로 복용이
가능하면서 환경오염도 막을 수 있는 IoT 스마트 약통을 생각해냈다.


## 2. 주요기능 및 전체 시스템 구성도

<img src = "https://github.com/buglossJisoo/IoT_Smart_Pill/assets/70942492/3de68f68-e682-423c-9699-9a4956a6fb0d">

1. 사용자 등록 기능
> 애플리케이션을 통해 사용자가 직접 나이, 성별, 키, 몸무게, 복용중인 약, 자신의 사진을 등록 할 수 있도록 하였으며, 이러한 사용자의 정보를 Firebase Realtime Database로 전송하는 기능

2. 약 복용 알림&복용체크
> 사용자가 사전에 등록한 복용시간대에 대한 약의 복용 알림 서비스를 제공해주며, 약을 섭취하였을 시 자동으로 복용 체크하는 기능

3. 사용자 인식&약 드롭
> 라즈베리파이와 웹 캠, facial recognition기술을 이용해 사용자를 인식하며, 인식된 사용자의 약을 서보모터를 이용해 드롭하도록 하는 기능

4. 추가 서비스
> 사용자가 등록한 약의 정보를 기반으로 동반 복용 시 위험 혹은 효과 없는 약의 정보를 제공하는 사용자 맞춤형 기능

5. 구매알림
> 사용자가 복용중인 약이 떨어지기 전에 구매를 권장하는 알림을 제공(구매를 권장하는 시점은 1주일전으로 설정)


## 3. 개발 시 사용한 주요 기술 및 하드웨어 

<img src = "https://github.com/buglossJisoo/IoT_Smart_Pill/assets/70942492/313dd2f6-16e6-4fd3-88af-2cc4f755dfe5">

1. Android Studio - Application
> 사용자, 약의 관한 정보들을 Firebase와 연동한 안드로이드 애플리케이션

2. Firebase - Database
> 애플리케이션을 통해 받아온 정보, 라즈베리파이에서 보내온 정보를 실시간으로 관리하기 위한 Firebase Realtime Database

3. Raspberry Pi - Facial Recognition
> 사용자의 사진 데이터셋을 이용한 Facial Recognition 기술을 Raspberry Pi와 웹 캡을 통해
기능 구현, 시연

4. 3D Printer - Drop the Pill
> 약을 드롭하는 기능을 구현하기 위해, 3D 프린터를 이용해 약 드롭 기능 하드웨어를 제작

## 4. 시연 영상

<https://youtu.be/pui2YZKG-1s>
