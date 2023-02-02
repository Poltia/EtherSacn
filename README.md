# EtherScan

#### React기반으로 Go-Ethereum을 활용해서 블록 생성 및 조회, 트랜잭션 조회 구현

#

<div align="center">
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
<img src="https://img.shields.io/badge/react_redux-764ABC?style=for-the-badge&logo=redux&logoColor=black">
</div>
<div align="center">
<img src="https://img.shields.io/badge/thunk-339933?style=for-the-badge&logo=node.js&logoColor=black">
<img src="https://img.shields.io/badge/react_router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=black">
</div>
<div align="center">
<img src="https://img.shields.io/badge/styled_components-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=black">
<img src="https://img.shields.io/badge/axios-5A29E4?style=for-the-badge&logo=axios&logoColor=black">
</div>
<div align="center">
<img src="https://img.shields.io/badge/express-000000?style=for-the-badge&logo=express&logoColor=white">
<img src="https://img.shields.io/badge/mysql2-4479A1?style=for-the-badge&logo=mysql&logoColor=black">
</div>
<div align="center">
<img src="https://img.shields.io/badge/sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=black">
<img src="https://img.shields.io/badge/web3.js-F16822?style=for-the-badge&logo=web3.js&logoColor=black">
</div>
<div align="center">
<img src="https://img.shields.io/badge/cors-339933?style=for-the-badge&logo=node.js&logoColor=black">
<img src="https://img.shields.io/badge/dotenv-ECD53F?style=for-the-badge&logo=dotenv&logoColor=black">
</div>

#

### 페이지 구성

- Main
  ![MainPage](https://raw.githubusercontent.com/Poltia/EtherSacn/main/imgs/Main.png)

  - 최신 블록 리스트를 실시간으로 출력.
  - 블록 정보 페이지로 이동할 수 있게 클릭 이벤트 구현
  - Mining Start 버튼으로 채굴 시작.
    <br/>클릭하면 Mining Stop 으로 버튼의 이름과 색상 변경.
  - 원하는 번호의 블록 검색/조회 기능 구현.
    <br/>
    <br/>
    <br/>

- Block
  ![BlockPage](https://raw.githubusercontent.com/Poltia/EtherSacn/main/imgs/Block.png)

  - 선택한 블록의 정보를 출력.
  - 아래 버튼 클릭시 해당 블록의 트랜잭션 목록을 출력.
    <br/>해당 트랜잭션의 정보를 보여주는 페이지로 넘어가는 클릭 이벤트 기능 구현.
    <br/>
    <br/>
    <br/>

- TxInfo
  ![TxInfoPage](https://raw.githubusercontent.com/Poltia/EtherSacn/main/imgs/TxInfo.png)
  - Block 페이지에서 선택한 트랜잭션의 정보를 출력.

#

### 이슈

- 이슈 : 버튼으로 채굴 시작/정지 구현하기
  - 해결
    <br>블록과 트랜잭션 정보는 web3.js를 사용해서 가져왔는데, 이부분은 web3.js로 구현할 수 없어서 axios로 요청을 보냄으로 해결
