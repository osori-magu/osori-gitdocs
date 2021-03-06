# Slack ChatBot

## Why? 

### 간단한 REST API를 주고 받는 웹개발에서 많이 사용됨

### 웹 서버이지만 API서버도 사용 가능 

  
기본적으로 Flask 프레임워크는 마이크로 서비스를 사용한느데 많이 사용하고요. Flask는 웹사이트가 아니더라도 간단한 API를 만드는데 많이 사용되요.   
  
그래서 서버를 구동하기 위해서 Flask가 필요하기도 한거에요.   
  
이제 우리는 TODO웹사이트를 만들어 볼거에요.   
거기에 Slack챗봇을 연동시켜 1\) slack명령어로 todo를 생성 2\) todo를 조회하는 기능을 만들어 볼거에요.   


## Slack chatbot 동작 원리 

![](../.gitbook/assets/image%20%28239%29.png)

1번 가장 왼쪽은 Flask 서버에요.  
2번 가장 아래 아이콘은 Slack  
3번 우측 상단은 slack의 chatbot이에요.    
  
기본적으로 slack에서 chatbot을 만들거에요.  


### chatbot에 2가지 등록 

1\)  웹 서비스에서 동작을 했을때 해당 동작이 있었다는 slack 알림받  
2\)  slack안에서 명령을 했을 때 반영하는 동작   
  
- command &lt; -&gt; URL의 경우 slack에서 명령어를 입력했을때 해당 URL을 연동해 줄 것을 요청하는 것이에요.   
- 그 안에서 URLs을 요청에 대한 응답으로 보내게되요. 그럼 slack에서 한 URL를 생성해요. 그 URL에다가 정보를 맞춰서 넣어주면 그게 메시지화되어 알람이 되요.   
  
다음 시간 slack사이트에 가입하고 원하는 기능을 구현해 보도록 할게요. 



