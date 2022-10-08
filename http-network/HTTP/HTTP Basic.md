# HTTP Basic

## 📌 Client와 Server 간에 통신

### ⚡️ **Client**: 리소스가 필요한 쪽
  - Request(요청) 송신
  - 반드시 Client에서 통신이 시작

### ⚡️ **Server**: 리소스를 제공하는 쪽
  - Response(응답) 송신
  - Request 받지 않고 Response를 송신 ❌

---

## 📌 Request와 Response

### ⚡️ Request
> GET /index.html HTTP /1.1 <br>
> Host: www.youtube.com 

<br>

#### GET (HTTP Method)
-  서버에 요구하는 작업의 종류

#### /index.html (Request Message)
- 요구 대상인 리소스

#### HTTP /1.1 (버전 정보)
- Client 기능을 식별하기 위함

#### 한 마디로..
> HTTP 서버 상에 있는 "index.html" 소스 좀 주소~
