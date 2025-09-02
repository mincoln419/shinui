# 시누이 앱 공식 웹사이트

시누이 앱의 공식 다운로드 페이지입니다.

## 🌐 라이브 사이트

**공식 웹사이트**: [https://mincoln419.github.io/shinui-website](https://mincoln419.github.io/shinui-website)

## 📱 시누이 앱 소개

**시누이**는 "시간을 누적하고 이정표를 세우다"라는 의미로, 귀여운 잔소리꾼 캐릭터와 함께하는 24시간 시간 관리 및 3줄 일기 앱입니다.

### 🌟 주요 기능

- **24시간 시간 관리**: 시간대별로 세밀하게 계획하고 실행하는 2단계 체크박스 시스템
- **3줄 일기**: 느낀점, 후회하는 점, 각오를 통해 하루를 되돌아보기
- **통계 및 분석**: 카테고리별 시간 분배와 완료율을 시각적으로 확인
- **템플릿 관리**: 개인 맞춤형 시간 관리 템플릿 생성 및 관리
- **캐릭터 시스템**: 시누냥(고양이)과 시누견(시바견) 중 선택 가능한 시간 코치

### 🎨 캐릭터

#### 🐱 시누냥 (고양이 코치)

- 츤데레 성격의 고양이 코치
- 툭툭 던지면서도 끝까지 챙겨주는 스타일
- 게으름을 경계하는 잔소리꾼이지만 속은 따뜻한 조언자

#### 🐶 시누견 (시바견 코치)

- 활발하고 직진형인 시바견 코치
- 열정 넘치는 cheerleader
- 적극적으로 밀어주는 트레이너 역할

## 🚀 다운로드

### Android

- Google Play Store에서 다운로드 (출시 예정)
- APK 파일 직접 다운로드 (개발자 버전)

### iOS

- App Store에서 다운로드 (출시 예정)
- TestFlight 베타 테스트 (제한적)

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: 반응형 디자인, Flexbox, Grid
- **JavaScript**: 바닐라 JS (ES6+)
- **GitHub Pages**: 정적 사이트 호스팅
- **Google Fonts**: Noto Sans KR 폰트

## 📁 프로젝트 구조

```
shinui-website/
├── index.html              # 메인 페이지
├── privacy.html            # 개인정보처리방침
├── terms.html              # 이용약관
├── _config.yml             # Jekyll 설정
├── _redirects              # 리다이렉트 설정
├── assets/
│   ├── icons/
│   │   ├── shinui-icon.png # 앱 아이콘
│   │   └── favicon.png     # 파비콘
│   └── images/
│       └── og-image.png    # 소셜 미디어 이미지
├── package.json            # Node.js 설정
├── .gitignore              # Git 무시 파일
└── README.md               # 프로젝트 설명
```

## 🚀 로컬 개발

### 요구사항

- Node.js 16+ (선택사항)
- Git

### 설치 및 실행

```bash
# 저장소 클론
git clone https://github.com/mincoln419/shinui-website.git
cd shinui-website

# 의존성 설치 (선택사항)
npm install

# 로컬 서버 실행 (선택사항)
npm start

# 또는 간단히 브라우저에서 index.html 열기
open index.html
```

## 📝 업데이트 가이드

### 다운로드 링크 업데이트

1. **Android APK 링크**:

   ```html
   <!-- docs/index.html에서 수정 -->
   <a
     href="https://github.com/mincoln419/shinui/releases/download/v1.0.0/shinui-v1.0.0.apk"
     class="download-btn android"
   ></a>
   ```

2. **iOS App Store 링크**:
   ```html
   <!-- docs/index.html에서 수정 -->
   <a
     href="https://apps.apple.com/app/shinui/id[앱ID]"
     class="download-btn ios"
   ></a>
   ```

### 앱 정보 업데이트

- **버전 정보**: `index.html`의 메타 태그 및 내용
- **스크린샷**: `assets/images/` 폴더에 추가
- **앱 설명**: `index.html`의 기능 설명 섹션

## 🎨 디자인 커스터마이징

### 색상 변경

```css
/* 메인 그라데이션 */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* 버튼 색상 */
.download-btn.android {
  background: linear-gradient(135deg, #3ddc84, #2bb673);
}

.download-btn.ios {
  background: linear-gradient(135deg, #007aff, #0056b3);
}
```

### 폰트 변경

Google Fonts에서 다른 폰트를 선택하고 `index.html`의 링크를 업데이트하세요.

## 📊 분석 및 모니터링

### Google Analytics 설정

```html
<!-- index.html에 추가 -->
<script
  async
  src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"
></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag() {
    dataLayer.push(arguments);
  }
  gtag("js", new Date());
  gtag("config", "GA_MEASUREMENT_ID");
</script>
```

## 🔧 GitHub Pages 설정

1. **Repository Settings** → **Pages**
2. **Source**: Deploy from a branch
3. **Branch**: main
4. **Folder**: / (root)

## 📞 문의 및 지원

- **이메일**: contact@codenyang.com
- **GitHub Issues**: [이슈 리포트](https://github.com/mincoln419/shinui-website/issues)
- **메인 앱 저장소**: [shinui](https://github.com/mincoln419/times_line)

## 📄 라이선스

MIT License - 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

---

© 2024 CodeNYang. All rights reserved.
