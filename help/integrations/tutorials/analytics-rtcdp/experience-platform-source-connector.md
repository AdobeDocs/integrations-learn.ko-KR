---
title: Experience [!DNL Platform] 소스 커넥터 튜토리얼과  [!DNL Analytics] 및 실시간 고객 데이터 [!DNL Platform] 통합
description: Experience [!DNL Platform] 소스 커넥터를 사용하여 Adobe [!DNL Analytics] 와 실시간 고객 데이터 [!DNL Platform] 를 통합하는 방법을 알아봅니다.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="통합" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
TQID: https://experienceleague.adobe.com/Uct30-UadP-2Ocwslbk-dMAV0Y2unZlA339hThnofpA
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 11%

---

# Adobe [!DNL Analytics] 및 실시간 고객 데이터 [!DNL Platform]을(를) Experience [!DNL Platform] 소스 커넥터와 통합

<ol>
    <li>데이터를 수집할 <a href="https://experienceleague.adobe.com/ko?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">스키마를 만듭니다</a>.</li>
    <li>데이터를 수집할 <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=ko" _target="_blank" rel="noopener noreferrer">데이터 세트를 만듭니다</a>.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=ko" _target="_blank" rel="noopener noreferrer">스키마에서 올바른 ID 및 ID 네임스페이스를 구성</a>하여 수집된 데이터를 통합 프로필에 연결할 수 있도록 합니다.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=ko-KR" _target="_blank" rel="noopener noreferrer">프로필에 대해 스키마와 데이터 세트를 사용하도록 설정</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=ko-KR" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] 소스 커넥터</a>를 사용하여 [!DNL Analytics] 데이터를 Experience Platform으로 수집합니다.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html?lang=ko" _target="_blank" rel="noopener noreferrer">경험 [!DNL Platform]에서 세그먼트를 만듭니다.</a> 시스템은 세그먼트가 배치(데이터 커넥터) 또는 스트리밍(Edge 네트워크)으로 평가되는지 여부를 자동으로 결정합니다.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=ko" _target="_blank" rel="noopener noreferrer">프로필 속성 및 대상자 멤버십을 원하는 대상에 공유하기 위한 대상을 구성합니다.</a></li>   
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics] 소스 커넥터에 대한 표준 워크플로 단계는 [!DNL Analytics]의 데이터를 &quot;있는 그대로&quot; 수집하는 데 사용되는 스키마 및 데이터 집합을 만듭니다. 따라서 처음 두 단계는 시스템에서 처리됩니다. 매핑 워크플로를 사용하려면 사용자 지정 속성을 만들어야 하므로 단계 순서를 따르십시오.
