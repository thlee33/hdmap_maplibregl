# Autopilot Vision Simulator (MapLibre GL JS)

정밀도로지도 데이터를 기반으로 자율주행 자동차의 1인칭 시점 내비게이션을 시뮬레이션하는 웹 애플리케이션입니다.

## 주요 기능
- **1인칭 주행 시뮬레이션:** 지정된 차선(Link)을 따라 차량 카메라 시점이 부드럽게 주행하며, 실제 속도감을 연출(비네팅 효과 및 HUD 속도계).
- **Turf.js 기반의 수학적 동기화:** 매 프레임 좌표의 방향(Bearing)을 계산하여 지도의 회전 및 차량 마커의 방향을 완벽하게 일치시킴.
- **PIP(Picture-in-Picture) 미니맵:** 화면 좌측 상단에 여의도 전체를 조망하는 미니맵(Region Overview) 오버레이 제공. 메인 지도의 주행 위치 및 방향과 지연 없이 실시간 동기화.
- **다크 테마 및 유리 질감 UI:** Glassmorphism 디자인 기법이 적용된 컨트롤 패널과 MapLibre Dark 타일 기반의 모던한 시각화 경험 제공.

## 기술 스택
- **Core:** React 18, Vite
- **Mapping Engine:** MapLibre GL JS
- **Geospatial Processing:** Turf.js
- **Data Format:** WGS84 GeoJSON

## 시작하기
```bash
# 종속성 설치
npm install

# 로컬 개발 서버 실행
npm run dev

# GitHub Pages 배포용 빌드 (../maplibre 폴더로 생성됨)
npm run build
```
