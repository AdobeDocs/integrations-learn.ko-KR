---
title: ' [!DNL Target] 자습서와  [!DNL Analytics] 통합'
description: Adobe [!DNL Analytics] 을(를) Adobe [!DNL Target]과(와) 통합하는 방법을 알아보세요.
solution: Analytics, Target
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
exl-id: 4ab6c61f-f14e-408a-a700-53f7b3d0600a
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 1%

---

# [!DNL Analytics]과(와) [!DNL Target] 통합


## 통합 값 및 설정

아래 비디오에는 이 통합을 사용할 때의 가치와 통합 설정에 대한 세부 사항이 나와 있습니다.

>[!NOTE]
>
>이 비디오에서는 [!DNL Target] at.js 및 [!DNL Analytics] appMeasurement.js에 대한 구현과 유효성 검사를 보여 줍니다. 두 도구의 필수 라이브러리 버전에 대해서는 [설명서](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4timplementation.html)를 참조하십시오.

### A4T([!DNL Target]의 경우 [!DNL Analytics]) 설정 중

이 비디오에서는 개발자를 대상으로 하며 다음 방법을 학습합니다.

* SDID를 사용하여 [!DNL Analytics] 및 [!DNL Target] 요청을 바인딩하는 방법 설명
* [!DNL Target] Adobe(A4T)를 사용하여 [!DNL Analytics] Adobe에 대한 구현 요구 사항 설명

>[!VIDEO](https://video.tv.adobe.com/v/35146/?quality=12&learn=on)

### [!DNL Target]에 대해 [!DNL Analytics]을(를) Data Source으로 사용

이 비디오에서는 비즈니스 전문가를 대상으로 다음을 학습합니다.

* A4T란 무엇이며 A4T를 사용하는 이유는 무엇입니까?
* A4T는 어떻게 작동합니까?
* A4T를 사용하기 위한 사전 요구 사항은 무엇입니까?

>[!VIDEO](https://video.tv.adobe.com/v/17384/?quality=12&learn=on)


## 일반적인 사용 사례

아래 비디오에서는 A4T를 통해 통합하는 다양한 기능, 활동 유형 및 이점을 보여 줍니다.

### Analysis Workspace의 [!DNL Target] (A4T) 패널에 대한 [!DNL Analytics]

[!DNL Target]용 [!DNL Analytics] (A4T) 패널을 사용하면 Analysis Workspace에서 자신 있게 Adobe [!DNL Target] 활동 및 경험을 분석할 수 있습니다.

>[!VIDEO](https://video.tv.adobe.com/v/37247/?quality=12&learn=on)

### A4T 패널을 사용하여 자동 [!DNL Target] 활동 분석

이 비디오에서는 [!DNL Target] 패널의 [!DNL Analytics]을(를) 사용하여 자동 [!DNL Target] 테스트의 결과를 시각화하는 방법에 대해 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/333270/?quality=12&learn=on)

또한 &quot;자동 할당&quot; 및 &quot;자동 타겟&quot; 활동을 위해 Analysis Workspace에서 A4T 보고서를 설정하는 방법에 대한 세부 사항을 보여주는 두 가지 단계별 자습서가 있습니다.

## 자동 할당 활동을 위해 Analysis Workspace에서 A4T 보고서 설정 {#a4t-auto-allocate}

자동 할당 활동은 둘 이상의 경험에서 승자를 식별하고, 테스트가 계속 실행되고 학습되는 동안 더 많은 트래픽을 승자에게 자동으로 재할당합니다. 자동 할당을 위한 [!DNL Target]용 [!DNL Analytics] (A4T) 통합을 사용하면 [!DNL Analytics] Adobe에서 보고 데이터를 볼 수 있으며, [!DNL Analytics]에 정의된 사용자 지정 이벤트 또는 지표에 최적화할 수도 있습니다.

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-allocate-activities.html" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">자동 할당 활동에 대한 A4T 보고서 설정</span>
</a>

## 자동 [!DNL Target] 활동을 위해 Analysis Workspace에서 A4T 보고서 설정 {#a4t-auto-target}

자동 [!DNL Target] 활동에 대한 [!DNL Target] (A4T) 통합용 [!DNL Analytics]은(는) Adobe [!DNL Target] ML(Ensemble Machine Learning) 알고리즘을 사용하여 Adobe [!DNL Analytics] 목표 지표를 사용하는 동안 각 방문자의 프로필, 동작 및 컨텍스트를 기반으로 최상의 경험을 선택합니다.

Adobe [!DNL Analytics] Analysis Workspace에서 다양한 분석 기능을 사용할 수 있지만 실험 활동(수동 A/B 테스트 및 자동 할당)과 개인화 활동(자동 [!DNL Target]) 간의 차이로 인해 자동 [!DNL Target] 활동을 올바르게 해석하려면 [!DNL Target] 패널의 기본값 [!DNL Analytics]을(를) 몇 가지 수정해야 합니다.

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-target-activities.html" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">자동 [!DNL Target] 활동에 대한 A4T 보고서 설정</span>
</a>
