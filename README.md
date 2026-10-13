# 🎸 VintageRiff Studio (빈티지리프 스튜디오)
> **아날로그 일렉기타 타브 악보 에디터 & 빈티지 앰프 사운드 엔진**

빈티지 진공관 앰프 헤드와 레트로 페달보드 감성을 그대로 담은 인터랙티브 일렉기타 타브 악보 웹 애플리케이션입니다.

---

## ⚡ Netlify 배포 가이드 (스타일 깨짐 방지 완벽 해결!)

Netlify 배포 시 **"그냥 글자만 보이는 현상"**은 보통 `index.html` 파일 1개만 단독으로 드래그 앤 드롭했거나, 하위 `css/`, `js/` 폴더가 함께 업로드되지 않았을 때 발생합니다.

본 프로젝트는 이 문제를 **원천 차단**하기 위해:
1. `index.html` 내부에 **모든 마스터 CSS 디자인 시스템을 인라인으로 완전 내장**하였습니다.
2. 따라서 **`index.html` 단일 파일만 Netlify에 올려도 100% 완벽한 디자인**으로 정상 작동합니다!

### 가장 쉬운 Netlify 배포 방법 2가지:

#### 방법 1: 폴더 통째로 드래그 앤 드롭 (가장 권장)
1. [Netlify](https://app.netlify.com/)에 로그인합니다.
2. 상단 메뉴의 **"Sites"**로 이동한 후 화면 하단의 **"Drag and drop your site output folder here"** 박스를 찾습니다.
3. 현재 프로젝트 폴더 전체 (`test` 폴더 전체)를 해당 박스에 끌어다 놓습니다.
4. 수 초 내에 즉시 고유한 라이브 URL로 배포가 완료됩니다!

#### 방법 2: 깃허브(GitHub) 레포지토리 연동
1. 본 프로젝트 파일들을 GitHub 저장소에 푸시합니다.
2. Netlify에서 **"Add new site" > "Import an existing project"** 클릭 후 해당 저장소를 선택합니다.
3. Build command는 비워두고 Publish directory는 기본값(`.`)으로 설정한 뒤 Deploy 버튼을 누르면 자동 배포됩니다.

---

## ✨ 핵심 기능

1. **커스텀 50W 진공관 앰프 헤드 (Custom 50W Tube Amp)**
   - 2개의 **12AX7 진공관 (Vacuum Tubes)**: 연주와 음표에 실시간 반응하여 뜨겁게 발광
   - **출력 VU 미터계 (Analog VU Meter)**: 연주되는 사운드에 맞춰 실시간으로 튕기는 바늘
   - 로터리 노브 (Volume, Overdrive, Tone, Reverb, Delay, Tempo) 마우스 드래그 조작 지원
2. **3대 아날로그 스톰프박스 페달보드 (Analog Pedalboard)**
   - **VINTAGE SCREAMER (Overdrive)**: 그린 바디, 레드 LED, 진공관 게인 오버드라이브
   - **ANALOG DELAY (Tape Echo)**: 골드 바디, 그린 LED, 테이프 에코 딜레이
   - **SPRING REVERB**: 코발트 블루 바디, 블루 LED, 풍성한 스프링 리버브
3. **22프렛 최고급 로즈우드 지판 (Vintage Rosewood Fretboard)**
   - 자개(Pearloid) 닷 인레이 (3, 5, 7, 9, 12, 15, 17, 19, 21프렛)
   - 4~6번 줄 와운드 황동 코일 및 1~3번 줄 실버 스틸 현 질감
   - 펜타토닉, 블루스 스케일(b5 포함), 내추럴 마이너 등 스케일 가이드 온오프
   - 지판 클릭 시 즉시 일렉기타 사운드 재생 & 악보에 음표 자동 입력
4. **인터랙티브 6현 타브 악보 에디터 (Interactive TAB Notation)**
   - 키보드 숫자키(0~24) 및 방향키를 통한 즉각적인 타브 입력
   - 벤딩(b), 슬라이드(/), 해머링(h), 풀링(p), 비브라토(~), 팜뮤트(P.M.), 데드노트(X) 주법 지원
   - 실시간 골드 레이저 플레이헤드 스위핑 & 메트로놈 클릭
   - 양장본 파치먼트 종이 테마 vs 다크 트위드 무대 테마 1클릭 전환
5. **록 명곡 프리셋 6종 내장**
   - Deep Purple - *Smoke on the Water*
   - Guns N' Roses - *Sweet Child O' Mine*
   - Led Zeppelin - *Stairway to Heaven*
   - AC/DC - *Back in Black*
   - Jimi Hendrix - *Purple Haze*
   - Nirvana - *Come As You Are*
6. **유틸리티 & 내보내기**
   - 록 기타 코드 도감 & 운지법 SVG 다이어그램 모음 (원클릭 악보 삽입)
   - ASCII 텍스트 타브 변환 및 외부 타브 불러오기 (Import/Export)
   - `.vtab` 프로젝트 파일 저장/불러오기 & 브라우저 자동저장
   - 인쇄 및 PDF 악보 출력 모드
