# mentoring-

1. 각자의 리덕스의 이해도가 없다. 그래서 페이지를 나누다 보니깐 길을 잃어 버린다.

서버의 처리하는 방법에 따라 클라이언트도 방법이 많다

기철님의 이해 안가는 포인트.
상세 페이지를 넘어 갔을때 get요청으로 데이터를 불러와야 하는데  이사람이 무슨 게시물인지 알고 데이터를 뿌려줘야 하는데 
url에 쿼리문을 사용하여 서버에 보내고 값을 찾아서 데이터를 클라이언트로 불러 오는 방법 이다 .


상세 페이지를 클릭하는 시점에 url을 통해서 서버에 쿼리를 보내줘야 한다.
그 다음 axios를 바


상세페이지 조회 

메인에서 카테고리 별로 페이지 데이터 불러오는 것은 

그 부분 끝나고 시간 남으면 댓글 좋아요를 하는 것으로 

떨어지는 상태에서 진행을 했는데 전체 적인 진행도 

api 명세서를 통하여 

나머지 부분은 다 상세 페이지 -> 게시글 삭제 까지 골로 잡고 그 다음으로 시간이 남으면 댓글 댓글에서도 작성 조회 

1번 상세페이지, 수정, 업데이트 - 최대한의 골

2번 댓글 작성,조회 - 못 할수도 있다 

웹 개발 종합반 로그인 - 로직은 거의 비슷하다  -> 새봄님의 코드를 보고 이야기 해 보기 

미들웨어에서 헤더를 정의를 하는 방식은 좋지 않다

로그인 

.then 전에 {api}는 api 명세서와 같아야 한다 .

header 부분이 있는 이유는 백앤드 분들의 일종의 약속 이라고 보면 된다.

리듀서에서 보면 로컬 스토리지에 담고 있는데 리듀서는 순수 함수를 담고 있어야 하는데 
외부 적인 것을 넣으면 안 좋다 

유저 정보는 보통 로컬 스토리지에 담는다 거기에 담으면 유저가 페이지를 나가도 남아 있다 

로그인 유지 관련 기능은 인터셉터 기능을 사용 하면 된다 

# 인터셉터 관련 공부를 할 것 !

.then(res) => {
  const token = res.date.ressult.token;,
  const userid = res.date.result.userid;,
  
  localStorage.setItem('token', user_info);
  alret('로그인에 성공하셨습니다')
  history.push('/')
  
  
구글링 => 리액트로 로그인 상태 유지 관련 찾기 

추천. 리덕스 무조껀 잡고 가야 한다 

git = cli로 쓰는 법 찾기 

리덕스 흐름도 

1.디스패치 작동이 되려면 -> 페이지 첫 시작 될때 미들웨어 에서 데이터를 받고 함수에 넣는다-> 액션 함수는 리듀서를 실행 시키는 함수 (액션 함수 안에 갈로는 데이터를 리스트로 바꿔주는 것) star-> action.payload.star 리듀서에 담는다 , draft는 이니셜 스테이츠  -> useSelector 

흐름도의 이해를 위해서는 어떻게 인자를 받아오고 사용되는지 알아야 한다 .

직접 만들어 보는게 제일 좋다, 간단하게 만들어 보아도 되니깐 전체적으로 혼자서 만들어 보아야 한다.


