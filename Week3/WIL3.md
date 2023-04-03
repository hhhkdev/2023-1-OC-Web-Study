
# **Git의 기본 명령어**

## 1. `add`(변경사항 저장)

다음 변경(Commit)을 기록할 때까지 변경분 모아놓는 작업

```
git add 파일명
git add .               // 전체 add
git add *.txt           // 모든 txt 파일 업로드
git add proj/apps/*/    // 디렉토리 업로드
git add --update        // 현재 git이 추적하고 있는 파일들만 add
```


## 2. `commit`(변경사항 확정)

```
git commit -m {commit_message}
```


## 3. `push`(원격 저장소에 commit된 파일들을 모두 업로드)
```
git push -u origin master
```


<br>

# **`git pull`과 `git fetch`의 차이점**

## 1. `git pull`
원격저장소에 있는 변경사항들을 로컬저장소로 가져와 합치는 명령어
로컬저장소에 변경내용을 병합
```
git pull
```

## 2. `git fetch`
원격저장소에 있는 변경사항들을 로컬저장소에 가져오기 전에 변경내용을 확인하고 싶은 경우에 사용하는 
```
git fetch {원격저장소 이름}
```
<br>

# **WIL Week3**

## 배운점
Github Desktop을 처음 이용해봄으로써 Git에 조금 더 편하게 접근함.

## 느낀점
Git은 결국 앞으로도 많이 쓰일텐데 기본 소양으로 갖춰야할 능력이기에 조금 더 사용 방법을 연습할 필요가 있지 않을까 싶음.