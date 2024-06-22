`Preview` 

- **팀 구성**: 대박징조 6인조
- **개요 :** 딥러닝을 활용한 반려묘의 안구 질환 진단 및 사용자를 고려한 다양한 맞춤 서비스를 제공하는 반려묘 헬스케어 웹 개발 프로젝트
- **역할** : 데이터 수집 & EDA & 전처리, Streamlit 대시보드 개발, 팀 단위의 Notion 워크스페이스 운영 및    배포 (기여도 20%)
- **성과 :** EDA를 통한 효율적인 **시각화 대시보드** 개발, 단계적인 모델링 고도화 작업을 통한 질병 예측 정확도 약 **28%** 증진

---

**참여 대회 & 결과 :** 멀티캠퍼스 PJT 경진대회 & 최우수상, 1위

**(1) Google Drive :** [프로젝트 코드 & 데이터 & 산출물](https://drive.google.com/drive/folders/1RG1aH1zDg7JXFbCUYY0hjtHBhdFjx_2F?usp=sharing)

**(2) Notion(팀) :**

[‘냥이의 하루 안냥’ 프로젝트](https://www.notion.so/78e739d2fd1540f8a55e33975b9a6462?pvs=21)

### 📋프로젝트 개요

---

딥러닝을 활용한 반려묘의 안구 질환 진단 및 사용자를 고려한 다양한 맞춤 서비스를 제공하는 반려묘 헬스케어   웹 개발 프로젝트

### 📊 분석 과정

---

`분석 방법` 

- 분석 언어

<aside>
✔️ Python

- Selenium 라이브러리와 카카오맵 & API를 활용한 전국 동물병원 정보 데이터 수집
    
    ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/231dc523-75a0-4fd4-862b-d998fb7ff6ce)

    
    - 카카오맵에서 한 번에 가져올 수 있는 데이터의 개수는 총 500개로 수집 과정에서의 **문제** 발생
        - 전국 지역명 & 동물 병원 키워드를 기준으로 분할 수집 후 가공, **문제** 해결
        - 서울 & 경기 지역은 동물병원 지점 개수가 1,000개 이상인 점을 참작하여 자치구 단위로 추출
        - 중복 지점 & 주소 데이터 삭제
- Pandas, Numpy, Matplotlib, Seaborn 라이브러리를 활용한 EDA 및 전처리 진행
    - 고양이 안구 데이터셋 (Json → csv 형식으로 변환)
        
        ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/66ccadab-fec6-4565-a792-5a47fe3b3bfe)

        - 데이터셋 변환을 위한 함수화 후 데이터프레임 구축
        - 질병 5종 & 고양이 종 24종
    - 홈페이지의 질병 선택 옵션 기능 활성화 과정에서 **문제** 발생
        - [age_mean], 평균 연령 Column 생성 & 내림차순 정렬
        - 각 질병별로 데이터셋 분할 후 csv 파일로 변환, **문제** 해결
            
            ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/545811ca-8f2f-46ea-99af-9b12e0f5bb50)

            
- Streamlit을 활용한 사용자의 입장을 고려한 웹 대시보드 구축
    - Seaborn 라이브러리와 고양이 안구 질병 데이터를 활용한 시각화 그래프 설계
    - 5개의 질병에 따른 각각의 인사이트 그래프 제공
        - 전체 질병 분포 비율
        - 각 질병별 성별 분포
        - 각 질병별 연령 분포
        - 각 질병이 발생하는 종별 평균 나이, 눈 위치
            
            ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/156dfae5-0097-40f7-a6b6-507bc252990d)

    - Folium 라이브러리를 활용한 전국 동물병원 지도 & 정보 시각화
        - Sqlit3 DB에 전국 동물병원 데이터셋 저장
        - 로그인한 회원만 서비스 이용 가능
        - 지역 & 세부 지역 선택 기능 제공
            
            ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/518f64ba-7138-4517-9b76-7e6bf1cafe98)

- Keras, Tensorflow 딥러닝 라이브러리를 활용한 모델 학습 & 질병 예측 서비스 제공
    - Gradcam을 통한 수치적인 모델 성능에 대한 직관적인 시각화 자료 제공
        - 안구 질병 예측 진단 기준에 맞기 위한 히트맵 차트 채택
            
            ![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/f6e397d6-723e-42aa-b49a-780ec3d97776)

</aside>

### 🎯 프로젝트 결과 (실제로 개발한 서비스)

---

<aside>
✔️ 대박징조팀이 만든 질병예측진단 서비스 접속 **링크**

- 회원제로 운영
- 로그인 정보
    - ID : hong1
    - Password : hong1
    - [**‘냥이의 하루 안냥’ 홈페이지**](https://limjs102412-pythonproject2-home-ijsfek.streamlit.app/)
    
- 프로젝트의 관한 개요 & 분석 과정 & 결과 등 상세 내용을 보실 수 있습니다.
    - [“냥이의 안냥” 프로젝트 보고서](https://www.notion.so/cab37e40d9ca42129ec38d9590347a8e?pvs=21)
    
</aside>

- 반려묘의 안구질환별 다양하고 직관적인 시각화 자료 제공
- 병원의 위치, 전화번호, 영업시간을 지도 시각화 형태로 제공
- 반려묘 질병 정보와 건강상식을 실시간으로 답변해주는 챗봇 서비스 제공
- 사료 급여량, 음수량, 몸무게, 놀이시간 등을 달력에 기록하여 통계 정보 제공
- 반려묘의 안구질환 진단 모델을 통해 안구질환의 유무를 확인한 후 구체적인 병명을 진단하는 AI 서비스 제공

### 🛫 아쉬운점, 향후 계획

---

- 인턴 채용 과정으로 분석에 오랜 시간이 소모되는 모델링 담당에서 하차한 점 → Gradcam 시각화 제안
- 서비스를 고양이 안구 질병에 관해서만 선별한 점 → 기존 데이터셋을 바탕으로 다른 부위 질병도 맞춤화하여 고도화
- 네이버 Clova API 서비스 제공 기간으로 챗봇 서비스 종료 → 추후 사업화를 진행할 시 재활성화 예정
- Streamlit 라이브러리의 호환성 문제로 BI 도구 사용이 어려운 점 → Seaborn 과 Matplotlib 라이브러리로 BI 도구 대체

### 🧭 직무에 기여할 수 있는 부분

---

- 팀 단위의 Notion 환경 구축 및 운영 도움
- Map & API를 활용한 특정 정보에 대한 웹 스크래핑 역량
- 단계적인 모델링을 통한 통계적 가설 검증 & 정확도 개선 관여
- 자사 서비스 사용자의 입장을 고려한 인사이트 도출 & 대시보드 구축 역량

### 📺 발표 자료
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/288a5218-05ef-415c-aafb-8c946db5c95d)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/6b734ff8-8896-4cc9-aca8-a8b2bf4a1293)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/0adcf0c7-6741-42a3-8884-a2435501cba8)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/2d5a1919-7f94-4bc8-bd2f-f03a198268e0)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/81139726-13ec-4f86-84b2-ba84fd2f28a8)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/eefbaae4-1a50-4f56-afb5-e04aacc13f63)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/af2f8d2f-c2d0-4546-8ef2-bcf0324d2dab)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/fceb8522-f827-4a36-9d71-373b13705e92)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/24705dad-06a3-4c39-80f0-eaef373bbe14)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/94663dc5-e3b0-4777-aed8-fc8b4d4c0056)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/5e59f1b1-f146-4fe3-a109-967698771cbd)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/cfaddcf9-a456-4262-817a-4eeb62a7a217)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/a7c3ff2d-a587-46f0-805c-43c6a6b93c66)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/edf562c8-5608-498a-8549-fccd25bcff38)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/8415765b-4f82-4e30-9615-6607a02d8e3e)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/7d07d1b8-6246-4d34-9f3c-5223ee4cd6fb)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/c9974297-fcef-40b5-b595-a0a98b45e5d1)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/9f336523-58d2-4b93-a50a-92c69755b7c7)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/aa296e21-62a3-4e0d-a93d-0aba860b490e)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/1b516f2e-b174-4f9a-af22-1df7d170d1ed)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/24ad9d3f-5a82-41d5-b326-8b903bf612c4)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/f961aac7-6a92-4a6b-a782-7ae9537148c3)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/a966125c-ee30-4c24-bd44-8e7dd48ec762)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/ed9ac1c1-ccf6-4635-827c-fa246b6734a8)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/c019b2b9-94ef-409a-a7b8-8d93b80f420a)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/ee557666-375c-437c-945d-3523120fe8e5)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/86758577-41be-449b-ad1d-70d854d12512)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/d79ede52-8b45-43ad-90d8-e9057553ebf0)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/33199aa4-cee3-4817-a85e-bf21a646b2cd)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/2908ae56-4a34-4c86-9210-e18534961122)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/a2f821da-4bd4-400d-81b1-790d8d330eb7)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/e5812397-8c86-4634-ac9e-caee92337cf1)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/f98ab420-4ac9-4844-ad70-e09a1bcde7b9)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/e34bffba-c61c-445a-9622-a6efa58d8fc5)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/e92b1f32-3c2a-4bb4-a884-9f0e5e98825a)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/6d5e389d-9f84-448e-aeb0-4f16a07fd168)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/cb8e760c-1799-4a89-a723-cdbf067b6fb6)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/a56f82e8-11a7-4678-b3b4-ec8cf546e3d0)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/b9c32ec8-61d0-493b-b8ab-74a12cddfe2e)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/2be2219d-2d2b-4472-8ea1-9bf8c098f7ea)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/b4b48db4-a484-4ec4-8d6f-b528aea946a0)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/99a4a6e6-c91f-490f-8adb-f8210c481800)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/54f02efa-ee12-4bfe-977e-29aa2b8fbb2d)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/0281716d-5427-4e57-bb0a-32f219f48a74)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/e597fff4-f92d-47ed-b4e0-7842af873b63)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/4dcc2fbf-fb05-40e4-9672-37ae6397158f)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/3b3d07ba-ab7d-4c65-81c0-f7649fea4f01)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/c61b3292-1117-48ab-868a-352b03fa9805)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/987b650d-0c04-4197-b253-7cb1b9ebf485)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/f298e1bb-e8ca-4443-b5e0-18a6e2a5f19d)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/474cfaa3-5cf8-4b2d-b3e0-1ae0147c39d2)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/89d992bf-eed7-4eb1-9d28-5d354de5d409)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/52d491ea-fa71-44cb-abdc-c9aabc4b67e1)
![image](https://github.com/YoungMinDA/Cat-Eye-Disease-Analysis-Diagnosis-Service-Project/assets/109095108/c6cb372d-43f4-44ff-a1b5-aa688cd1dce9)
