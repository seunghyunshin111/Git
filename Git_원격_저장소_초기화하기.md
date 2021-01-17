## Git_원격 저장소 초기화하기

<br>

1. 로컬에 존재하는 .git 디렉토리를 삭제한다.

   ~~~c
   rm -rf ./.git
   ~~~

2. git init을 다시 수행하여 초기화 한다

   ~~~python
   git init
   
   # 결과메시지
   /www/.git/ 안의 빈 깃 저장소를 다시 초기화했습니다.
   ~~~

3. 현재 상태로 커밋한다.

   ~~~
   git add .
   git commit -m 'commit message'
   ~~~

4. 원격 저장소를 연결한다.

   ~~~python
   git remote add origin <url>
   
   # 잘 되었는지 확인한다.
   git remote -v
   
   # 결과메시지
   origin Git-Address (fetch)
   origin Git-Address (push)
   ~~~

5. 현재 상태를 원격저장소에 적용한다.

   ~~~python
   git push origin master
   
   # 안 될 경우
   git push --force --set-upstream origin master
   ~~~

   

