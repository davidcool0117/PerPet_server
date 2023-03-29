![header](https://user-images.githubusercontent.com/117795271/228464367-27ec4951-d265-45c3-ae7d-595ca3d46636.png)

---

# **📌 About**

#### Front에서 상품정보를 받아 각각의 페이지에 정보를 전달합니다.

- 메인페이지(hotdeal)
- 메인페이지(이상품어때?)
- 상품 상세 페이지

# 🛠 Stack

![Nodejs][node-image]&nbsp;&nbsp;&nbsp;![Express][express-image] ![Sequelize][sequelize-image] ![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

---

# **🙏 Request**

### 상품 정보 요청

| **페이지** |                                **RequestURL**                                | **Format** |                                                                     **통신방식**                                                                      |
| :--------: | :--------------------------------------------------------------------------: | :--------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: |
| 메인페이지 |   https://port-0-perpetserver-p8xrq2mlfc5j4rt.sel3.cloudtype.app/products    |  **JSON**  | <span style="background-color: #339933; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">get</span> |
| 상세페이지 | https://port-0-perpetserver-p8xrq2mlfc5j4rt.sel3.cloudtype.app/products/{id} |  **JSON**  | <span style="background-color: #339933; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">get</span> |

### 상품 업로드

|  **페이지**  |                             **RequestURL**                              | **Format** |                                                                      **통신방식**                                                                      |
| :----------: | :---------------------------------------------------------------------: | :--------: | :----------------------------------------------------------------------------------------------------------------------------------------------------: |
| 업로드페이지 | https://port-0-perpetserver-p8xrq2mlfc5j4rt.sel3.cloudtype.app/products |  **JSON**  | <span style="background-color: #CB3837; display:inline-block; width: 50px; height: 26px; border-radius:5px;color:white; text-align:center">post</span> |

[express-image]: https://img.shields.io/badge/express-000000?style=for-the-badge&logo=express&logoColor=white
[pwa-image]: https://img.shields.io/badge/pwa-6109AC?style=for-the-badge&logo=pwa&logoColor=white
[sequelize-image]: https://img.shields.io/badge/sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=white
[node-image]: https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white
[npm-image]: https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white
