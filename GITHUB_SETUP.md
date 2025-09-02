# GitHub Repository 설정 가이드

시누이 웹사이트를 GitHub Pages로 배포하기 위한 설정 가이드입니다.

## 🚀 1단계: GitHub Repository 생성

### GitHub에서 새 Repository 생성

1. **GitHub.com**에 로그인
2. **"New repository"** 클릭
3. **Repository 설정**:
   - **Repository name**: `shinui-website`
   - **Description**: `시누이 앱 공식 웹사이트 - GitHub Pages`
   - **Visibility**: `Public` ✅
   - **Initialize**: 체크하지 않음 (이미 파일이 있음)

## 🔗 2단계: Remote Repository 연결

```bash
# 현재 디렉토리에서 실행
git remote add origin https://github.com/[YOUR_USERNAME]/shinui-website.git

# 예시 (실제 사용자명으로 변경)
git remote add origin https://github.com/mincoln419/shinui-website.git
```

## 📤 3단계: 코드 업로드

```bash
# 첫 번째 푸시
git push -u origin main
```

## ⚙️ 4단계: GitHub Pages 활성화

1. **Repository 페이지**에서 **"Settings"** 탭 클릭
2. 왼쪽 메뉴에서 **"Pages"** 클릭
3. **Source** 섹션에서:
   - **Deploy from a branch** 선택
   - **Branch**: `main` 선택
   - **Folder**: `/ (root)` 선택
4. **"Save"** 클릭

## 🌐 5단계: 사이트 접속

배포가 완료되면 다음 URL로 접속할 수 있습니다:

- **기본 URL**: `https://[YOUR_USERNAME].github.io/shinui-website`
- **예시**: `https://mincoln419.github.io/shinui-website`

## 🔄 6단계: 자동 배포 확인

- `main` 브랜치에 푸시할 때마다 자동으로 GitHub Pages에 배포됩니다
- 배포 상태는 **"Actions"** 탭에서 확인할 수 있습니다

## 📝 7단계: 커스터마이징

### 다운로드 링크 업데이트

1. **Android APK 링크**:

   ```html
   <!-- index.html에서 수정 -->
   <a
     href="https://github.com/[YOUR_USERNAME]/shinui/releases/download/v1.0.0/shinui-v1.0.0.apk"
     class="download-btn android"
   ></a>
   ```

2. **iOS App Store 링크**:
   ```html
   <!-- index.html에서 수정 -->
   <a
     href="https://apps.apple.com/app/shinui/id[앱ID]"
     class="download-btn ios"
   ></a>
   ```

### 메타 태그 업데이트

```html
<!-- index.html에서 수정 -->
<meta
  property="og:url"
  content="https://[YOUR_USERNAME].github.io/shinui-website"
/>
<meta
  property="og:image"
  content="https://[YOUR_USERNAME].github.io/shinui-website/assets/images/og-image.png"
/>
```

## 🎨 8단계: 디자인 커스터마이징

### 색상 변경

```css
/* index.html의 <style> 섹션에서 수정 */
body {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

### 로고 변경

1. `assets/icons/shinui-icon.png` 파일 교체
2. `assets/icons/favicon.png` 파일 교체

## 📊 9단계: 분석 도구 추가 (선택사항)

### Google Analytics

```html
<!-- index.html의 <head> 섹션에 추가 -->
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

## 🔧 문제 해결

### 배포가 안 될 때

1. **Actions 탭**에서 에러 로그 확인
2. **Settings > Pages**에서 설정 재확인
3. 파일 경로 및 권한 확인

### 이미지가 안 보일 때

1. 파일 경로 확인 (`assets/` 폴더)
2. 파일명에 특수문자 없는지 확인
3. 파일 크기 확인 (너무 크지 않은지)

## 📞 지원

문제가 발생하면:

1. **GitHub Issues**에 문제 보고
2. **이메일**: contact@codenyang.com

---

이제 시누이 앱의 공식 웹사이트가 GitHub Pages에서 호스팅됩니다! 🎉
