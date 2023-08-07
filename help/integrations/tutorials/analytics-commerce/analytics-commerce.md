---
title: 통합 [!DNL Analytics] 포함 [!DNL Commerce] 튜토리얼
description: 통합 방법 알아보기 [!DNL Analytics] 포함 [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="통합" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 5%

---


# 통합 [!DNL Analytics] 포함 [!DNL Commerce]

## 초기 온보딩

이 지침은 Adobe 용입니다. [!DNL Commerce] 클라우드 호스팅 프로젝트. 자체 호스팅은 어느 정도 달라질 수 있지만 전체 프로세스는 유사해야 합니다.

1. 로컬 환경에서 코드 체크 아웃
1. 작성기 사용 및 설치 모듈
1. 여기에서 개별 지침을 따르고 완료되면 돌아가서 나머지 단계를 완료합니다
   [경험 설치 및 구성 [!DNL Platform] 커넥터](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. composer.json을 커밋하고 클라우드에 composer.lock 파일이 있는 경우
1. 모듈이 스테이징 및/또는 프로덕션 환경에 있는지 확인합니다. Adobe의 관리 섹션에 로그인하면 됩니다. [!DNL Commerce] 및 시스템 > 서비스에서 이러한 새 섹션 찾기
   ![경험 [!DNL Platform] 커넥터 확장](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Adobe 내에서 자격 증명으로 모듈을 구성합니다 [!DNL Commerce] 백 오피스.
   * 첫 번째 [!DNL Commerce] 아래 표시된 대로 서비스 커넥터 구성
     ![[!DNL Commerce] 서비스 커넥터 설정](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 그런 다음 경험 [!DNL Platform] 아래 표시된 커넥터 설정.
     ![경험 [!DNL Platform] 커넥터](./assets/analytics-commerce/experience-platform-connector.png)

온보딩 프로세스의 각 단계 및 단계에 대한 자세한 내용은 [경험 [!DNL Platform] 커넥터 개요](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. 경험 [!DNL Platform] 커넥터 튜토리얼에서는 각 섹션을 자세히 살펴보고 질문에 답변합니다. 나머지 빠른 설정 단계는 이 자습서를 사용하십시오.

## Experience Edge 및 Adobe 구성 [!DNL Analytics]

1. 조직에 Adobe 액세스 권한이 있는지(및 사용자에게 권한이 있는지) 확인합니다. [!DNL Analytics]. 다음으로 이동하여 이를 확인할 수 있습니다. [Adobe Experience Cloud 홈 페이지](https://experience.adobe.com/) 위쪽 탐색에서 애플리케이션 전환기(9개 점)를 클릭합니다.

1. Adobe에서 새 보고서 세트 만들기 [!DNL Analytics]또는 푸시할 보고서 세트의 ID를 식별합니다 [!DNL Commerce] 데이터 입력. 자세한 내용은 다음 튜토리얼을 참조하십시오. [새 보고서 세트 만들기](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=ko). 아래 데이터 스트림 단계에서 이 보고서 세트 ID가 필요합니다.

1. 다음 위치로 이동 [Adobe 경험 [!DNL Platform] 인터페이스](https://platform.adobe.com) experience에 액세스할 수 있는 경우 [!DNL Platform]. 해당 인터페이스에 액세스할 수 없는 경우 Adobe Experience에서 아래에 나열된 필요한 모든 단계를 수행할 수 있습니다 [!DNL Platform] [데이터 수집 인터페이스](https://experience.adobe.com/#/data-collection).

1. 를 사용하여 XDM 스키마 생성 또는 업데이트 [!DNL Commerce]-특정 필드 그룹. 스키마를 만드는 방법에 대한 자세한 내용은 [&quot;스키마 만들기&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html) 튜토리얼.
   * 아래 데이터 스트림 단계의 옵션에서 이 스키마를 선택해야 합니다. 스키마를 만들려면 아래의 왼쪽 열을 살펴보십시오. **데이터 관리** 및 찾기 **스키마**. 이제 인터페이스의 오른쪽 상단에서 **스키마 만들기**. XDM ExperienceEvent 를 선택합니다.
   * 새 스키마를 만들면 [!DNL Commerce] 필드 그룹. UI의 왼쪽에서 필드 그룹을 찾아 **추가**
      * 검색에서 다음을 입력하여 필터링할 수 있습니다. `ExperienceEvent [!DNL Commerce]`
      * 다음 항목 선택 **Adobe [!DNL Analytics] 경험 이벤트[!DNL Commerce]** 확인란을 선택하여
      * 그런 다음 **필드 그룹 추가** 저장하고 계속하기 위해 오른쪽 상단

1. 선택 사항(그리고 환경에 있는 경우에만) [!DNL Platform] 인터페이스) - 새 데이터 세트 만들기
   * 이 단계에서는 다음을 가져올 수 있습니다. [!DNL Commerce] 경험으로의 데이터 [!DNL Platform] (데이터를 Adobe으로 가져오는 것과 별도로) [!DNL Analytics]). 경험에 액세스할 수 있는 경우 이 단계를 수행하십시오 [!DNL Platform]및 은(는) 다음을 사용할 계획입니다. [!DNL Commerce] 경험의 데이터 [!DNL Platform]실시간 고객 데이터와 같은 애플리케이션 지원 [!DNL Platform], 고객 여정 [!DNL Analytics]또는 Journey Optimizer.
   * 아래 데이터 스트림 단계의 옵션에서 이 데이터 세트를 선택해야 합니다.
   * 왼쪽 열 아래 **데이터 관리** 왼쪽 탐색에서 제목 을 선택합니다. **데이터 세트**.
   * 클릭 **데이터 세트 만들기** 오른쪽 상단에서 다음을 선택합니다. **스키마에서 데이터 세트 만들기** 옵션을 선택합니다.
   * 마지막 단계에서 생성한 스키마를 검색하고 사용합니다

1. 전송할 데이터 스트림 만들기 [!DNL Commerce] Adobe 데이터 [!DNL Analytics]
   * 아래 **데이터 수집** 왼쪽 열에서 제목 을 선택합니다. **데이터스트림**.
   * 클릭 **새 데이터스트림** 인터페이스 오른쪽 상단에서
   * 이름 및 설명(선택 사항)을 입력합니다.
   * 이전 단계에서 생성/식별한 스키마를 찾아 선택합니다.
   * 원하는 고급 옵션을 추가합니다. 고급 옵션에 대한 자세한 내용은 [설명서](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=ko-KR).
   * 클릭 **저장** 계속합니다.
   * 클릭 **서비스 추가** 및 선택 **Adobe[!DNL Analytics]** 을 클릭합니다.
   * 클릭 **보고서 세트 추가** 이전 단계에서 생성/식별한 보고서 세트 ID를 입력합니다. 데이터가 여러 보고서 세트로 흘러들어가도록 하려면 보고서 세트를 두 개 이상 추가할 수 있습니다.
   * 필요한 경우 이전 단계에서 데이터 세트를 만든 경우 **서비스 추가** 다시, 선택 **Adobe 경험[!DNL Platform]** 을 클릭합니다. 이벤트 데이터 세트 필드에서 이전에 만든 데이터 세트를 선택합니다.
   * 데이터스트림을 저장합니다.

1. 마지막으로, [!DNL Commerce] 데이터, Adobe의 Analysis Workspace으로 이동해야 합니다. [!DNL Analytics], 프로젝트를 만들고, 보고서 세트를 선택하고, 자유 형식 테이블 및 기타 시각화를 추가하여 [!DNL Commerce] 데이터. 다음 이미지는 Analysis Workspace에서 만들 수 있는 표의 예를 보여 줍니다.

   ![[!DNL Analytics] 일부 상거래 데이터의 스크린샷](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   다음은 Analysis Workspace에서 작업하는 데 도움이 되는 몇 가지 추가 리소스입니다.

   * [Analysis Workspace 개요](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [처음부터 새로 작업 영역 프로젝트 빌드](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Analysis Workspace에서 표, 시각화 및 패널 사용](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [시각화 사용 사례](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   또한 Experience League 시 무료 강좌도 제공됩니다. 다음을 참조하십시오 [!DNL Analytics] 사용 가능한 강의 [여기](https://experienceleague.adobe.com/?lang=en&amp;Solution=[!DNL Analytics]#courses).
