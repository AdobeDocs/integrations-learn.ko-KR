---
title: ' [!DNL Commerce] 자습서와  [!DNL Analytics] 통합'
description: ' [!DNL Analytics] 을(를)  [!DNL Commerce]과(와) 통합하는 방법을 알아봅니다.'
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
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# [!DNL Analytics]과(와) [!DNL Commerce] 통합

## 초기 온보딩

이 지침은 [!DNL Commerce] Cloud 호스팅 프로젝트 Adobe에 사용됩니다. 자체 호스팅은 어느 정도 달라질 수 있지만 전체 프로세스는 유사해야 합니다.

1. 로컬 환경에서 코드 체크 아웃
1. 작성기 사용 및 설치 모듈
1. 여기에서 개별 지침을 따르고 완료되면 돌아가서 나머지 단계를 완료합니다
   [경험 설치 및 구성 [!DNL Platform] 커넥터](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html?lang=ko){target="_blank"}


1. composer.json을 커밋하고 클라우드에 composer.lock 파일이 있는 경우
1. 모듈이 스테이징 및/또는 프로덕션 환경에 있는지 확인합니다.
[!DNL Commerce] Adobe의 관리 섹션에 로그인한 다음 시스템 > 서비스에서 새 섹션을 찾아 이 작업을 수행할 수 있습니다
   ![Experience [!DNL Platform] 커넥터 확장](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. [!DNL Commerce] 백 오피스 Adobe 내에서 자격 증명을 사용하여 모듈을 구성합니다.
   * 아래에 표시된 대로 먼저 [!DNL Commerce] 서비스 커넥터 구성을 사용합니다.

     ![[!DNL Commerce] 서비스 커넥터 설정](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 그런 다음 아래 표시된 대로 Experience [!DNL Platform] 커넥터 설정을 사용합니다.

     ![경험 [!DNL Platform] 커넥터](./assets/analytics-commerce/experience-platform-connector.png)

온보딩 프로세스의 각 단계 및 단계에 대한 자세한 내용은 [경험 [!DNL Platform] 커넥터 개요](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html?lang=ko){target="_blank"}의 지침을 따르십시오. Experience [!DNL Platform] 커넥터 튜토리얼은 각 섹션에 대해 자세히 설명하고 있을 수 있는 질문에 답합니다. 나머지 빠른 설정 단계는 이 자습서를 사용하십시오.

## Experience Edge 및 Adobe [!DNL Analytics]의 구성

1. 조직에 [!DNL Analytics] Adobe에 대한 액세스 권한이 있는지 확인하십시오. [Adobe Experience Cloud 홈 페이지](https://experience.adobe.com/)(으)로 이동하여 위쪽 탐색에서 응용 프로그램 전환기(9개 점)를 클릭하면 확인할 수 있습니다.

1. [!DNL Analytics] Adobe에서 새 보고서 세트를 만들거나 [!DNL Commerce] 데이터를 푸시할 보고서 세트의 ID를 식별합니다. 자세한 정보는 [새 보고서 세트 만들기](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=ko)에 대한 자습서를 참조하십시오. 아래 데이터 스트림 단계에서 이 보고서 세트 ID가 필요합니다.

1. [!DNL Platform] Adobe에 액세스할 수 있는 경우 [경험 관리 [!DNL Platform] 인터페이스](https://platform.adobe.com)(으)로 이동합니다. 해당 인터페이스에 액세스할 수 없는 경우 Adobe 환경 [!DNL Platform] [데이터 수집 인터페이스](https://experience.adobe.com/#/data-collection)에서 아래 나열된 필요한 모든 단계를 수행할 수 있습니다.

1. [!DNL Commerce]별 필드 그룹으로 XDM 스키마를 만들거나 업데이트합니다. 스키마를 만드는 방법에 대한 자세한 내용은 [&quot;스키마 만들기&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=ko) 자습서를 참조하십시오.
   * 아래 데이터 스트림 단계의 옵션에서 이 스키마를 선택해야 합니다. 스키마를 만들려면 **데이터 관리**&#x200B;의 왼쪽 열에서 **스키마**&#x200B;를 찾습니다. 이제 인터페이스 오른쪽 상단에서 **스키마 만들기**&#x200B;를 클릭합니다. XDM ExperienceEvent 를 선택합니다.
   * 새 스키마를 만든 후 [!DNL Commerce] 필드 그룹을 추가합니다. UI의 왼쪽에서 필드 그룹을 찾아 **추가**&#x200B;를 클릭합니다
      * 검색에서 `ExperienceEvent Commerce`을(를) 입력하여 필터링할 수 있습니다.
      * 확인란을 선택하여 **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]**&#x200B;을(를) 선택하십시오.
      * 그런 다음 오른쪽 상단의 **필드 그룹 추가**&#x200B;를 클릭하여 저장하고 계속합니다

1. 필요한 경우(그리고 Experience [!DNL Platform] 인터페이스인 경우에만) - 새 데이터 세트를 만듭니다.
   * 이 단계에서는 [!DNL Analytics] Adobe으로 데이터를 가져오는 것과 별도로 [!DNL Commerce] 데이터를 [!DNL Platform] 경험으로 가져올 수 있습니다. [!DNL Platform] 경험에 액세스할 수 있고 Real-Time Customer Data [!DNL Platform], 고객 여정 [!DNL Analytics] 또는 Journey Optimizer과 같은 Experience [!DNL Platform] 지원 응용 프로그램에서 [!DNL Commerce] 데이터를 사용할 계획인 경우 이 단계를 수행합니다.
   * 아래 데이터 스트림 단계의 옵션에서 이 데이터 세트를 선택해야 합니다.
   * 왼쪽 탐색 메뉴의 왼쪽 열 **데이터 관리** 머리글 아래에서 **데이터 세트**&#x200B;를 선택합니다.
   * 오른쪽 상단의 **데이터 집합 만들기**&#x200B;를 클릭합니다. **스키마에서 데이터 집합 만들기** 옵션을 선택하십시오.
   * 마지막 단계에서 생성한 스키마를 검색하고 사용합니다

1. [!DNL Commerce] 데이터를 Adobe [!DNL Analytics] (으)로 보낼 데이터 스트림을 만드십시오.
   * 왼쪽 열의 **데이터 수집** 제목 아래에서 **데이터스트림**&#x200B;을 선택합니다.
   * 인터페이스 오른쪽 상단에서 **새 데이터스트림**&#x200B;을 클릭합니다.
   * 이름 및 설명(선택 사항)을 입력합니다.
   * 이전 단계에서 생성/식별한 스키마를 찾아 선택합니다.
   * 원하는 고급 옵션을 추가합니다. 고급 옵션에 대한 자세한 내용은 [설명서](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=ko-KR)를 참조하십시오.
   * 계속하려면 **저장**&#x200B;을 클릭하세요.
   * **서비스 추가**&#x200B;를 클릭하고 드롭다운 필드에서 **Adobe[!DNL Analytics]**&#x200B;을(를) 선택합니다.
   * **보고서 세트 추가**&#x200B;를 클릭하고 이전 단계에서 생성/식별한 보고서 세트 ID를 입력합니다. 데이터가 여러 보고서 세트로 흘러들어가도록 하려면 보고서 세트를 두 개 이상 추가할 수 있습니다.
   * 필요한 경우 이전 단계에서 데이터 세트를 만든 경우 **서비스 추가**&#x200B;를 다시 클릭하고 드롭다운 필드에서 **경험 Adobe[!DNL Platform]**&#x200B;을(를) 선택합니다. 이벤트 데이터 세트 필드에서 이전에 만든 데이터 세트를 선택합니다.
   * 데이터스트림을 저장합니다.

1. 마지막으로 [!DNL Commerce] 데이터를 보려면 Adobe [!DNL Analytics]에서 Analysis Workspace으로 이동하여 프로젝트를 만들고, 보고서 세트를 선택하고, 자유 형식 테이블 및 기타 시각화를 추가하여 [!DNL Commerce] 데이터를 보고하고 분석해야 합니다. 다음 이미지는 Analysis Workspace에서 만들 수 있는 표의 예를 보여 줍니다.

   일부 상거래 데이터의 ![[!DNL Analytics] 스크린샷](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   다음은 Analysis Workspace에서 작업하는 데 도움이 되는 몇 가지 추가 리소스입니다.

   * [Analysis Workspace 개요](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html?lang=ko)
   * [처음부터 Workspace 프로젝트 빌드](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html?lang=ko)
   * [Analysis Workspace에서 표, 시각화 및 패널 사용](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html?lang=ko)
   * [시각화 사용 사례](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html?lang=ko)

   또한 Experience League 시 무료 강좌도 제공됩니다. [여기](https://experienceleague.adobe.com/ko?lang=en&amp;Solution=Analytics#courses)에서 사용 가능한 [!DNL Analytics] 과정을 참조하세요.
