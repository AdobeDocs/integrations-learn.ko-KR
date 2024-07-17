---
title: Experience [!DNL Platform] 소스 커넥터 자습서와  [!DNL Analytics] 및 고객 여정 [!DNL Analytics] 통합
description: Experience [!DNL Platform] 소스 커넥터를 사용하여 Adobe [!DNL Analytics] 을 고객 여정 [!DNL Analytics] 과 통합하는 방법을 알아봅니다.
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="통합" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# Adobe [!DNL Analytics] 및 고객 여정 [!DNL Analytics]을(를) Experience [!DNL Platform] 소스 커넥터와 통합

<ol>
    <li>데이터를 수집할 <a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">스키마를 만듭니다</a>.</li>
    <li>데이터를 수집할 <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">데이터 세트를 만듭니다</a>.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">스키마에서 올바른 ID 및 ID 네임스페이스를 구성</a>하여 수집된 데이터를 통합 프로필에 연결할 수 있도록 합니다.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=ko-KR" _target="_blank" rel="noopener noreferrer">프로필에 대해 스키마와 데이터 세트를 사용하도록 설정</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] 원본 커넥터</a>를 사용하여 [!DNL Platform] 경험에 데이터 수집</li>
    <li><i>(선택 사항)</i>. 여러 데이터 세트를 사용하는 경우 개인 ID를 함께 <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">결합된 데이터 세트를 생성</a>합니다. 단일 [!DNL Analytics] 데이터 세트를 사용하거나 고객 여정 [!DNL Analytics]에서 사용하려는 모든 데이터 세트에 공통 식별자가 있는 경우 이 단계를 건너뜁니다.</li>
    <li>고객 여정 [!DNL Analytics]에서 <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">연결을 만듭니다</a>.</li>
    <li>고객 여정 [!DNL Analytics]에서 <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">데이터 보기 만들기</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">구성 요소 설정 구성</a> 및 <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">서식 지표</a>.
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=ko-KR" _target="_blank" rel="noopener noreferrer">고객 여정 [!DNL Analytics]에서 프로젝트를 만듭니다.</a></li>
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics] 원본 커넥터에 대한 표준 워크플로 단계는 [!DNL Analytics]의 데이터를 &quot;있는 그대로&quot; 수집하는 데 사용되는 스키마 및 데이터 집합을 만듭니다. 따라서 처음 두 단계는 시스템에서 처리됩니다. 매핑 워크플로를 사용하려면 사용자 지정 속성을 만들어야 하므로 단계 순서를 따르십시오.
