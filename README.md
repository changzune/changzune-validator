# ChangzuneValidator

SAP 스타일의 통합 유효성 검사기.  
입력된 데이터가 DB에 저장되기 전에 @ValidString, @ValidDate 등의 애노테이션을 통해  
**타입, 형식, 길이, 공백 여부 등 다양한 조건을 검증**하고,  
조건을 만족하지 않으면 저장 자체를 차단합니다.

---

## 💡 주요 기능

- `@ValidString`: 문자열 길이, 공백 여부 검증
- `@ValidDate`: 날짜 포맷 및 과거/미래 날짜 제한
- `ValidationEngine`: 서비스 단에서 수동 호출 가능한 검증 유틸

---

## ⚙️ 설치 방법 (JitPack 기준)

```groovy
repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.changzune:changzune-validator:0.1.0-SNAPSHOT'
}