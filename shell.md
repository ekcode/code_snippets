# 각종 명령어

### keytool

JRE에 등록된 CA 리스트 확인

`$JAVA_HOME/jre/lib/security ➜  keytool -list -keystore cacerts`

CA 추가

`$JAVA_HOME/jre/lib/security ➜  keytool -keystore cacerts -importcert -alias comodorsa -file comodorsa.cer`


### ncdu

디스크 사용량 확인

`du -sh *` 보다 빠르고 한눈에 들어온다.


### lsof -n -i :3000

3000번 포트를 사용 중인 PID
