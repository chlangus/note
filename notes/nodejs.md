## nodejs
+ 웹 브라우저 바깥에서 자바스크립트를 실행하는 환경
+ API를 제공하는 프로그램은 웹 브라우저 바깥에서 실행됨
<br/>

## Express
+ 자바스크립트 백엔드 개발쪽에서 가장 유명한 라이브러리
+ 리퀘스트와 리스폰스를 쉽게 다룰 수 있음
+ 다른 라이브러리에 비해 특정 구조를 고집하지 않고 최소한의 기능들만 제공함
+ const app = express();
+ app.method(path, handler)구조로 사용    
  ex) app.get('/some/path', (req, res)=> { // 리퀘스트 처리 })
<br/>


## Mongo DB
+ 데이터를 테이블에 저장하지 않고 문서 형태로 저장
+ 문서하나 = 도큐먼트
+ 문서의 모음 = 컬렉션
+ 셋업 과정도 간단하고 도큐먼트 다루는 방법 직관적 

<br/>
## json
+ res.send에 의해 javascript 객체가 json형식으로 변환 
