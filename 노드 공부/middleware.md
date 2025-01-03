⚙️ [미들웨어 함수]
클라이언트에게 요청이 오고 그 요청을 보내기 위해 응답하려는 중간(미들)의 목적에 맞게 처리를 하는, 거쳐가는 함수들

미들웨어 함수는 req(요청), res(응답)객체, 그리고 어플리케이션 요청-응답 사이클 도중 그 다음의 미들웨어 함수에 대한 엑세스 권한을 가지는 함수이다.

다음 미들웨어 함수에 대한 엑세스는 next 함수를 이용해서 다음 미들웨어로 현재 요청을 넘길 수 있다.

next를 통해 미들웨어는 순차적으로 처리된다.

- app.get()
  사용 방법: app.get("경로", callback[,callback...])

⚙️ [req, res]
응답 객체- respone
res.app: 똑같이 res 객체를 통해 app 객체에 접근한다. res.app.get('')같이 사용 가능.

각 라우터에 반드시 한번만 써야되는 것
res.end()
res.json(JSON)
res.redirect(주소)
res.render(뷰, 데이터)
res.send(데이터)
res.sendFile(경로)

요청 객체 = request
req.app: req 객체를 통한 app 객체로의 접근이다.

