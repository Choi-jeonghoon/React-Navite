# React Native Expo 학습 기록

## 1. 프로젝트 개요
이 프로젝트는 React Native와 Expo를 사용하여 모바일 앱을 개발하는 과정을 학습한 기록입니다. 주로 스타일 적용, 클릭 이벤트 처리, iOS와 Android 간의 차이점을 다루었습니다.

---

## 2. 주요 학습 내용

### 2.1. 스타일 적용
- React Native에서 스타일은 `StyleSheet` 객체를 사용하여 적용합니다. 각 컴포넌트에 직접 스타일을 적용하거나, 객체 형태로 스타일을 정의할 수 있습니다.

```javascript
const styles = StyleSheet.create({
  textInput: {
    borderWidth: 1,
    borderColor: "#cccccc",
    width: "100%",
    padding: 8,
    color: "white", // 텍스트 색상
  },
});
```

### 2.2. 클릭 이벤트 처리
- React Native에서는 onPress 속성을 사용하여 클릭 이벤트를 처리할 수 있습니다. 주로 버튼 컴포넌트, 텍스트 컴포넌트에서 사용됩니다.

```javascript
<Button title="클릭하세요" onPress={handleClick} />
```
- onPress: 사용자가 버튼을 클릭했을 때 호출되는 함수

### 2.3. iOS와 Android 간의 차이점
- React Native는 iOS와 Android 간의 플랫폼 차이를 고려하여 UI를 구성해야 합니다. 다음은 학습한 주요 차이점입니다.

iOS:

- 네비게이션 바가 기본적으로 투명하게 설정되어 있습니다.
- 폰트 및 UI 요소들이 기본적으로 작고 깔끔한 디자인을 가지고 있습니다.

Android:
- 네비게이션 바가 불투명하며 더 큰 텍스트와 UI를 사용하는 경향이 있습니다.
- 백 버튼이 기본적으로 존재하여 앱의 내비게이션 동작이 다를 수 있습니다.


### 2.4. 메인 페이지의 배경화면 설정

Expo로 프로젝트를 생성한 후, `app.json` 파일에 아래와 같이 `backgroundColor` 속성을 추가하면 모든 페이지의 배경화면 색상을 일괄적으로 설정할 수 있습니다(단, 모달 창은 제외됩니다).

```json
{
  "expo": {
    "backgroundColor": "#1e085a"
  }
}
```
- 이후 추가 코드 설명 및 내용은 아래 노션에 따로 기록을 남겨놨습니다.

https://www.notion.so/React-native-Code-108e533a426d80c5a10fea362be45432?pvs=4
