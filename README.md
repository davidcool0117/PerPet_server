<div align="center">
<img width="329" alt="image" src="https://user-images.githubusercontent.com/117795271/228409021-d39db6a9-7b40-4630-b779-5739818d0102.svg">
</div>

---

# 📌 About

#### Restful 방식으로 Front에서 상품정보를 받아 각각의 페이지에 정보를 전달합니다.

**메인페이지(hotdeal)
메인페이지(이상품어때?)
상품 상세 페이지**

---

# 🛠 Stack

![Nodejs][node-image]&nbsp;&nbsp;&nbsp;![Express][express-image] ![Sequelize][sequelize-image] ![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

---

# 📥 Install

### Backend

```bash
$ git clone https://github.com/wooyoung6685/perpetserver.git
$ cd perpetserver
```

```bash
$ nvm use v.16.19.0
$ npm init
$ npm i cors
$ npm i express
$ npm i multer
$ npm i nodemon
$ npm i sequelize
$ npm i sqlite3
$ npm start
```

---

# **🙏 Request**

**API : RESTFUL API**
**Data Type : JSON**

<span style="background-color: #339933; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">get</span> /products 상품 정보 조회

<span style="background-color: #CB3837; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">post</span> /products 상품 등록

<span style="background-color: #339933; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">get</span> /products/id 상품 상세 페이지

| Parameter key |  Data정보  | NULL |
| :-----------: | :--------: | :--: |
|      ID       |    ID값    |  X   |
|     NAME      |   상품명   |  X   |
|    SELLER     |   판매자   |  X   |
|   ORGPRICE    |    원가    |  X   |
|     PRICE     |   할인가   |  O   |
|   DISCOUNT    |   할인율   |  O   |
|  DESCRIPTION  |  상품정보  |  X   |
|     IMAGE     | 이미지주소 |  X   |
|    SOLDOUT    | 품절 유무  |  X   |

[express-image]: https://img.shields.io/badge/express-000000?style=for-the-badge&logo=express&logoColor=white
[pwa-image]: https://img.shields.io/badge/pwa-6109AC?style=for-the-badge&logo=pwa&logoColor=white
[sequelize-image]: https://img.shields.io/badge/sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=white
[node-image]: https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white
[npm-image]: https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white
