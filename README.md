<!--
사용 방법:
1) GitHub에서 자기 계정명과 동일한 이름의 새 저장소를 만듭니다. 예) GeonHoong/GeonHoong
2) 그 저장소의 README.md에 이 파일 내용을 그대로 붙여넣으면 프로필 페이지 상단에 표시됩니다.
3) <> 로 표시된 부분(이름/링크/이메일 등)을 본인 정보로 교체하세요.
-->

<div align="center">

# 안녕하세요, 김건홍입니다 👋
**하드웨어 × 임베디드 × 실시간 제어**를 다루는 자율주행 엔지니어입니다.

[![Email](https://img.shields.io/badge/Email-<your_email>-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:<your_email>)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-<your_handle>-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/<your_handle>)
[![Blog](https://img.shields.io/badge/Blog-<your_blog>-000000?style=flat-square&logo=github&logoColor=white)](https://<your_blog>)

</div>

---

## 🧭 About Me

- 🏎️ **1/10 스케일 자율주행 RC카** 프로젝트에서 **하드웨어 설계 총괄 + 실시간 제어 시스템**을 담당했습니다.
- 🔧 Autodesk Inventor로 섀시를 설계하고, ROS 2 ↔ micro-ROS ↔ OpenCR로 이어지는 제어 파이프라인을 직접 구축했습니다.
- 🧠 센서 데이터(카메라/LiDAR)를 실제 모터 명령까지 안전하게 연결하는 **제어 로직·안전 게이팅** 설계에 관심이 많습니다.

---

## 🛠 Tech Stack

![ROS2](https://img.shields.io/badge/ROS%202-22314E?style=flat-square&logo=ros&logoColor=white)
![micro-ROS](https://img.shields.io/badge/micro--ROS-1E8449?style=flat-square)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=C%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=Linux&logoColor=black)
![Arduino](https://img.shields.io/badge/OpenCR-00979D?style=flat-square&logo=arduino&logoColor=white)
![Inventor](https://img.shields.io/badge/Autodesk%20Inventor-D0021B?style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white)

---

## 🚀 Featured Project — 1/10 자율주행 RC카

> ROS 2 기반 차선 인식 · LiDAR 인지 · Pure Pursuit 제어를 통합한 자율주행 스택.
> 하드웨어 설계부터 임베디드 모터 제어까지 담당했습니다.

| 담당 영역 | 핵심 내용 |
|---|---|
| **MUX 통합 제어 노드** | 자율주행/조이스틱 명령을 0.6초 타임아웃 기반으로 중재해 50Hz로 단일 명령 발행. 페일세이프 자동 복귀 |
| **micro-ROS(OpenCR) 실시간 모터 제어** | PC(ROS 2) ↔ OpenCR 임베디드 보드를 micro-ROS 시리얼 브리지로 연결한 폐루프 제어 아키텍처 구축 |
| **LiDAR Lookahead 동적 조정 & ROI 가변 제어** | 차선 곡률·속도에 따라 Pure Pursuit Lookahead 거리와 LiDAR 인식 ROI(사각형 ↔ 부채꼴)를 실시간 연동, 근접 위험 시 비상정지 게이팅 |

```mermaid
flowchart LR
    CAM["카메라 · 차선 인식"] --> PP["Pure Pursuit\n(동적 Lookahead)"]
    LID["LiDAR · ROI 가변 인지"] --> PP
    JOY["조이스틱"] --> MUX["MUX 통합 제어"]
    PP --> MUX
    MUX -->|micro-ROS| OPENCR["OpenCR 모터/조향 구동"]
```

🔗 프로젝트 저장소: [<repo_url>](<repo_url>)

---

## 📊 GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=<your_username>&show_icons=true&theme=default&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=<your_username>&layout=compact&hide_border=true)

</div>
