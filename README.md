
<!-- head -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=청년&nbsp;사회성&nbsp;증대를&nbsp;위한&nbsp;모임&nbsp;추천&nbsp;서비스&fontSize=42" />
</p>

<!-- body -->

**기술 스택**
- *Spring FramWork 활용*
- *Java / JavaScript / AJAX*
- *HTML / CSS / JSP*
- *MySQL DB*
- *Python / COLAB / Pycharm*
  


---
<br/>

  **담당**

- 사진 등록 기능 구현(파일 선택, 미리 보기, Drag and Drop)
- 친구 추천 알고리즘 생성
- 친구 추천 관련 MySQL DB 관리,  추가
- 친구 추천 관련 페이지  JavaScript Ajax를 활용한 비동기 처리
- 친구 리스트 출력, 동아리 조회 페이지 리스트 출력 기능 구현
- 닮은 동물 상 찾기 모델(데이터 크롤링, 전처리, 모델링)

 --- 

<br/>

  **화면구현**
  
<br/>

- 사진등록 페이지
<br/>

![10Minutes시연영상](https://github.com/jeonggyohoon/Spring-AJAX-10MINUTES/assets/133930245/a260a05b-2fc5-4f07-b0cc-89fba82cbb39)

> code location
>> views / make_profile.jsp  
<br/>

- 닮은 동물상 결과 페이지
<br/>

![10Minutes시연영상 (1)](https://github.com/jeonggyohoon/Spring-AJAX-10MINUTES/assets/133930245/4ee9d20d-e14c-43bc-b6c4-71af3c682ae0)

> code location
>> views / view_result_profile_animal.jsp 
<br/>

- 친구 찾기 알고리즘, 리스트 출력 페이지
<br/>

![10Minutes시연영상 (3)](https://github.com/jeonggyohoon/Spring-AJAX-10MINUTES/assets/133930245/ac342945-3c3e-4803-b412-7f237fe8c97f)

> code location
>> views / view_friendSearch.jsp<br/>
>> views / m_list.jsp<br/>
>> views / f_list.jsp
<br/>

- 동아리 검색, 리스트 출력
<br/>

<p align="center">

![10Minutes시연영상 (6)](https://github.com/jeonggyohoon/MVC-pattern-imarket/assets/133930245/f8a18239-c253-46ad-8805-2d81d8a27bf2)

</p>

> code location
>> views / view_circleSearch.jsp<br/>
>> circle_List.jsp

<br/>

- 유사 동물상 찾기 모델링
<br/>

<p align="center">

![10Minutes시연영상 (5)](https://github.com/jeonggyohoon/MVC-pattern-imarket/assets/133930245/20e5e672-47b7-486a-9cf5-27585b39d88e)

</p>

> code location
>> use_model.py

<br/>

---

**comment**

- AJAX 비동기 리스트 출력 시 .jsp로 리스트 값을 바로 보내 <c:foreach>사용에 어려움이 있었다.


![1](https://github.com/jeonggyohoon/Spring-AJAX-10MINUTES/assets/133930245/884b4479-a248-4d0e-ab7f-0a5fa6acd37d)

#### 1. 비동기 처리 서버의 작업 순서가 JAVA>JSTL>HTML>JavaScript 이기 때문에 에러가 뜬다.

![2](https://github.com/jeonggyohoon/MVC-pattern-imarket/assets/133930245/45e66edd-11ac-43ed-9368-7ccb652c8a0b)

#### 2. JSP 상 출력할 위치를 잡아준 후 ajax에서 받아온 데이터를 다른 jsp에 그려서 그 그려진 jsp를 뿌려주는 방식을 사용했다.

<br/>

![3](https://github.com/jeonggyohoon/MVC-pattern-imarket/assets/133930245/0eded7fb-cfe7-486f-ad86-173e3c82a73e)

#### 3. controller 에서 return 위치에 jsp를 그릴 위치의 경로를 잡아 리스트를 보내주어야 한다.

![4](https://github.com/jeonggyohoon/MVC-pattern-imarket/assets/133930245/8e7780de-31f0-4b6f-a755-5ba73521f764)
