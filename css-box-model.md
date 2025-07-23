# CSS 박스 모델 정리

## Box Model 구성요소
- **margin (마진)**: 요소 바깥 여백
- **border (보더)**: 요소 테두리
- **padding (패딩)**: 콘텐츠와 테두리 사이의 여백
- **content (콘텐츠)**: 실제 내용이 들어가는 영역


---

## padding
- **콘텐츠(content)와 border 사이의 내부 여백**
- 요소의 **안쪽 공간을 확보**함

## margin
- **border 바깥쪽의 외부 여백**
- 요소 간의 **간격(거리)** 확보

---

## 마진/패딩 단축 속성

| 작성 방식 | 적용 순서 |
|-----------|------------|
| `margin: 20px;` | 4면 모두 20px |
| `margin: 20px 10px;` | 상하 20px, 좌우 10px |
| `margin: 20px 15px 5px 10px;` | 상 20px, 우 15px, 하 5px, 좌 10px (↪️ 시계방향) |

+패딩도 동일한 방식으로 사용 `padding: ...`

---

## box-sizing: border-box

- 기본값: `content-box`
  → 지정한 `width/height`는 content만 적용됨  
  → padding/border가 **밖으로 부풀면서** 전체 크기 증가

- `border-box`로 설정 시:
  → 지정한 `width/height` 안에  
  → **padding과 border까지 포함**됨  
  → ❗📌**원래 설정한 크기를 유지하면서** 안쪽에서 공간 확보됨


처음엔 margin이 padding이랑 헷갈렸는데, 정리하고 나니 딱 구분됨
💡상우하좌 순서, 상의하자로 외워서 적용하는 팁 기억하기

