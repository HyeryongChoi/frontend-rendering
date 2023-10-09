<p align="middle" >
  <img width="100px;" src="https://em-content.zobj.net/thumbs/160/apple/81/artist-palette_1f3a8.png"/>
</p>
<h2 align="middle">프론트엔드의 렌더링 방식</h2>
<p align="middle">내 서비스의 클론 코딩을 통해 프론트엔드 렌더링 방식 이해하기</p>
<br/>

![프론트엔드렌더링_미션_실행화면](https://github.com/woowacourse/frontend-rendering/assets/24777828/27946ad7-ff4e-4adc-8d7d-ff27629a4b04)

## 👀 클론 페이지 vs 원본 페이지

https://github.com/woowacourse/frontend-rendering/assets/24777828/4ce82a7f-722a-49f9-9036-04f30c44eb24

## 🎨 1단계 - 팀 서비스의 일부 페이지 클론 코딩

### 🚀 구현한 페이지의 주소와 방식

- 주소: [집사의고민 클론 페이지](https://frontend-rendering-kappa.vercel.app/)
- 렌더링 방식: SSG

### ✅ 선택한 렌더링 방식의 이유

이번 미션에서 클론 코딩한 페이지는 [집사의고민](https://zipgo.pet)의 메인페이지입니다.

사용자가 웹사이트를 처음 방문할 때 가장 먼저 보게 되는 중요한 페이지이기 때문에 선택했습니다.

메인페이지에서는 사료 목록을 확인할 수 있는데, 이 데이터는 변경이 거의 없기 때문에 SSG 렌더링 방식이 적합하다고 판단했습니다.

SSG방식은 프로젝트 빌드 시 미리 페이지를 사전에 렌더링하여 생성합니다. 이 페이지를 만들 때 필요한 데이터 또한 빌드 시점에 가져오게 됩니다.(fetching과정이 클라이언트 측 요청 시가 아니라 빌드 시 실행)

즉, 해당 페이지에 대한 요청이 발생했을 때 페이지를 동적으로 생성하는 게 아니라 이미 생성된 페이지를 정적으로 반환하는 형태로 동작합니다. 따라서 사용자들은 페이지 로딩 시 로딩 아이콘이 깜빡이는 현상 없이 더 빠르게 응답을 받을 수 있습니다.
