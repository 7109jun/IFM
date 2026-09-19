#  IFM Tag Engine

> **IFM Tag Engine**은 가벼운 커스텀 마크업 문법(`[IFM]`)을 사용하여 웹페이지나 마크다운 문서에 동영상, 오디오, 이미지 등의 미디어를 쉽고 직관적으로 임베드할 수 있는 초경량 파서 엔진입니다.

---

## 빠른 시작 (Quick Start)

1. 배포된 [웹사이트](https://7109jun.github.io/IFM/)에 접속합니다.
2. 아무거나 하세요
---

## 문법 안내 (Syntax Guide)

모든 IFM 태그는 대괄호(`[...]`) 안에 `data`와 `set` 속성을 지정하는 방식으로 작성합니다.

[IFM data="미디어_URL_또는_유튜브ID" set="동작모드"]

###  지원하는 동작 모드 (`set`)

| 모드 값 (`set`) | 설명 | 지원하는 미디어 |
| :--- | :--- | :--- |
| `video` | 소리와 함께 일반 재생 | 유튜브, MP4/WebM 동영상 |
| `mute` | 음소거 상태로 자동 재생 (루프) | 유튜브, MP4/WebM 동영상 |
| `audio` | 오디오 스트리밍 플레이어 표시 | MP3 등 오디오 파일 |
| `image` | 이미지 그래픽 출력 | JPG, PNG, WEBP 등 이미지 |

---

##  사용 예시 (Examples)

### 1. 일반 동영상 재생 (`set="video"`)
[IFM data="[https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4](https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4)" set="video"]

### 2. 음소거 자동 재생 배경 영상 (`set="mute"`)
[IFM data="[https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4](https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4)" set="mute"]

### 3. 오디오 스트림 재생 (`set="audio"`)
[IFM data="[https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3](https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3)" set="audio"]

### 4. 이미지 출력 (`set="image"`)
[IFM data="[https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?q=80&w=1000](https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?q=80&w=1000)" set="image"]
