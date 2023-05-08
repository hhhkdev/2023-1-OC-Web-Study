# 6주차

[[웹 기초 스터디 6주차 과제]](https://www.gdschongik.com/web-study/subject)

### 2023년 05월 09일 00시까지

**`Flexbox Froggy` 정답**

```css
// 1번 개구리를 오른쪽으로 이동시킴.
#pond {
  display: flex;
	**justify-content: flex-end;**
}

// 2번 개구리들을 수련잎으로 이동시킴.
#pond {
  display: flex;
	**justify-content: center;**
}

// 3번 세마리의 개구리를 수련잎 위로 이동. 수련잎 사이에 약간 간격이 있음.
#pond {
  display: flex;
	**justify-content: space-around;**
}

// 4번 수련잎 사이의 간격이 넓어짐. 동일한 간격이 존재함.
#pond {
  display: flex;
	**justify-content: space-between;**
}
```

```css
// 5번 개구리를 연못 아래쪽에 도착할 수 있도록 함.
#pond {
  display: flex;
	**align-items: flex-end;**
}

// 6번 연못의 중앙으로 이동시킴.
#pond {
  display: flex;
	**justify-content: center;
	align-items: center;**
}

// 7번 연못 아래쪽에, 주위에 간격이 있도록 함.
#pond {
  display: flex;
	**justify-content: space-around;
	align-items: flex-end;**
}
```

```css
// 8번 개구리를 좌우 반전시켜 배치함.
#pond {
  display: flex;
	**flex-direction: row-reverse;**
} 

// 9번 요소를 아래에서 위로 정렬함.
#pond {
  display: flex;
	**flex-direction: column;**
}

// 10번 요소를 오른쪽으로 보내고, 좌우 반전시킴.
#pond {
  display: flex;
	**flex-direction: row-reverse;
	justify-content: flex-end;**
}

// 11번 요소를 세로로 정렬하고 아래로 이동시킴.
#pond {
  display: flex;
	**flex-direction: column;
	justify-content: flex-end;**
}

// 12번 세로 반전시켜서 일정한 간격이 있도록 배치함.
#pond {
  display: flex;
	**flex-direction: column-reverse;
	justify-content: space-between;**
}

// 13번
#pond {
  display: flex;
	**flex-direction: row-reverse;
	justify-content: center;
	align-items: flex-end;**
}
```

```css
// 14번
#pond {
  display: flex;
}
.yellow {
	**order: 1;**
}

// 15번
#pond {
  display: flex;
}
.red {
	**order: -3;**
}

// 16번
#pond {
  display: flex;
  align-items: flex-start;
}
.yellow {
	**align-self: flex-end;**
}

// 17번
#pond {
  display: flex;
  align-items: flex-start;
}
.yellow {
	**order: 1;
	align-self: flex-end;**
}
```

```css
// 18번
#pond {
  display: flex;
	**flex-wrap: wrap;**
}

// 19번
#pond {
  display: flex;
	**flex-direction: column;
	flex-wrap: wrap;**
}

// 20번
#pond {
  display: flex;
	**flex-flow: column wrap;**
}
```

```css
// 21번
#pond {
  display: flex;
  flex-wrap: wrap;
	**align-content: flex-start;**
}

// 22번
#pond {
  display: flex;
  flex-wrap: wrap;
	**align-content: flex-end;**
}

// 23번
#pond {
  display: flex;
  flex-wrap: wrap;
	**flex-direction: column-reverse;
	align-content: center;**
}
```

```css
// 24번
#pond {
  display: flex;
	**flex-direction: column-reverse;
	flex-wrap: wrap-reverse;
	justify-content: center;
	align-content: space-between;**
}
```

# `flex-container`

- `flex-direction`: flex 컨테이너의 주축 방향을 설정함
    - `row row-reverse column column-reverse`
- `flex-wrap`: flex 컨테이너의 복수 flex item을 배치할 행 수를 결정함
    - `nowrap wrap wrap-reverse`
- `flex-flow`: flex-direction과 flex-wrap을 설정하기 위한 shorthand
    - `<flex-direction> || <flex-wrap>`
- `justify-content`: main axis를 기준으로 flex item을 수평 정렬함
    - `flex-start flex-end center space-between space-around`
- `align-items`: cross axis 방향으로 flex item을 수직 정렬함
    - `stretch flex-start flex-end center baseline`
- `align-content`: cross axis를 기준으로 flex item을 수직 정렬함
    - `stretch flex-start flex-end center space-between spacd-around`