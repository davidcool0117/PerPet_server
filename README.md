![header](https://user-images.githubusercontent.com/117795271/228464367-27ec4951-d265-45c3-ae7d-595ca3d46636.png)

![Nodejs][node-image]&nbsp;&nbsp;&nbsp;![Express][express-image] ![Sequelize][sequelize-image] ![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

# **📌 About**

여러 가지 플랫폼의 웹툰에 대한 정보를 제공하며 정보는 한시간 간격으로 갱신됩니다.

현재 정보가 제공되는 웹툰 플랫폼은 다음과 같습니다.

- 네이버웹툰
- 카카오웹툰
- 카카오페이지

# **🙏 Request**

## **웹툰 정보 요청**

조건을 만족하는 웹툰 정보들을 제공합니다.

| Method |                                     Request URL                                      | Format |
| :----: | :----------------------------------------------------------------------------------: | :----: |
|  GET   | [`https://korea-webtoon-api.herokuapp.com`](https://korea-webtoon-api.herokuapp.com) |  JSON  |

### **Request Parameter**

|     Name      | Required |  Type  | Default | Description                                                                                                                                                                                                   |
| :-----------: | :------: | :----: | :-----: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   **page**    |    N     | number |    0    | 페이지 번호                                                                                                                                                                                                   |
|  **perPage**  |    N     | number |   10    | 한 페이지 결과 수                                                                                                                                                                                             |
|  **service**  |    N     | string |    -    | 웹툰 공급자<ul><li>`naver` 네이버 웹툰</li><li>`kakao` 카카오 웹툰</li><li>`kakaoPage` 카카오페이지</li></ul>                                                                                                 |
| **updateDay** |    N     | string |    -    | 웹툰 업데이트 구분<ul><li>`mon` 월</li><li>`tue` 화</li><li>`wed` 수</li><li>`thu` 목</li><li>`fri` 금</li><li>`sat` 토</li><li>`sun` 일</li><li>`finished` 완결</li><li>`naverDaily` 네이버 Daily+</li></ul> |

### Response Sample

**https://korea-webtoon-api.herokuapp.com/?perPage=1&page=3&service=kakao&updateDay=sun**

```json
{
  "totalWebtoonCount": 5430,
  "naverWebtoonCount": 2032,
  "kakaoWebtoonCount": 1542,
  "kakaoPageWebtoonCount": 1856,
  "updatedWebtoonCount": 56,
  "createdWebtoonCount": 0,
  "lastUpdate": "2022-12-01T00:41:49.961Z",
  "webtoons": [
    {
      "_id": "638250d60d980db259c72c02",
      "webtoonId": 2000000003093,
      "title": "스포일러 보는 드라마 작가",
      "author": "원아",
      "url": "https://webtoon.kakao.com/content/스포일러-보는-드라마-작가/3093",
      "img": "https://kr-a.kakaopagecdn.com/P/C/3093/c1/2x/b973723c-39bb-4d69-b614-1b07ba82e2f6.png",
      "service": "kakao",
      "updateDays": ["sun"],
      "fanCount": null,
      "searchKeyword": "스포일러보는드라마작가원아",
      "additional": {
        "new": true,
        "rest": false,
        "up": true,
        "adult": false,
        "singularityList": []
      }
    }
  ]
}
```

## **웹툰 검색**

대소문자, 특수문자를 구분하지 않는 특정 키워드를 포함한 제목, 작가를 가진 웹툰 정보를 제공합니다.

| Method |                                            Request URL                                             | Format |
| :----: | :------------------------------------------------------------------------------------------------: | :----: |
|  GET   | [`https://korea-webtoon-api.herokuapp.com/search`](https://korea-webtoon-api.herokuapp.com/search) |  JSON  |

### **Request Parameter**

|    Name     | Required |  Type  | Default | Description |
| :---------: | :------: | :----: | :-----: | ----------- |
| **keyword** |    Y     | string |    -    | 검색 키워드 |

### Response Sample

**https://korea-webtoon-api.herokuapp.com/search?keyword=갓오브하이스쿨**

```json
{
  "totalWebtoonCount": 5430,
  "naverWebtoonCount": 2032,
  "kakaoWebtoonCount": 1542,
  "kakaoPageWebtoonCount": 1856,
  "updatedWebtoonCount": 43,
  "createdWebtoonCount": 0,
  "lastUpdate": "2022-12-01T01:41:51.421Z",
  "webtoons": [
    {
      "_id": "63824f5799624044b9326032",
      "webtoonId": 1000000318995,
      "title": "갓 오브 하이스쿨",
      "author": "박용제",
      "url": "https://m.comic.naver.com/webtoon/list?titleId=318995",
      "img": "https://image-comic.pstatic.net/webtoon/318995/thumbnail/thumbnail_IMAG21_38f18e00-09f2-4a0c-b36a-3aa56dfe0b3b.jpg",
      "service": "naver",
      "updateDays": ["finished"],
      "fanCount": 100,
      "searchKeyword": "갓오브하이스쿨박용제",
      "additional": {
        "new": false,
        "adult": false,
        "rest": false,
        "up": false,
        "singularityList": []
      }
    }
  ]
}
```

[express-image]: https://img.shields.io/badge/express-000000?style=for-the-badge&logo=express&logoColor=white
[pwa-image]: https://img.shields.io/badge/pwa-6109AC?style=for-the-badge&logo=pwa&logoColor=white
[sequelize-image]: https://img.shields.io/badge/sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=white
[node-image]: https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white
[npm-image]: https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white
