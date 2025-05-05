---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# [!DNL Analytics] 및 Audience Manager 통합

{{analytics-description}}

{{audience-manager-description}}

Adobe [!DNL Analytics] 데이터를 서버측에서 Audience Manager으로 전달하여 이 통합을 활성화하면 Audience Manager에게 데이터의 주요 소스 중 하나, 즉 온라인 고객 행동 데이터를 제공합니다. 그런 다음 이 데이터를 자사 CRM 데이터 또는 타사 파트너 데이터와 같은 다른 데이터와 결합하여 풍부한 고객 세그먼트를 만들 수 있습니다. 또한 이후 추가적인 방문자 분석에 대한 응답으로 Audience Manager 세그먼트는 웹 페이지로 다시 전송됩니다. 이러한 두 가지 중요한 사용 사례는 아래에 설명되어 있습니다.

Adobe [!DNL Analytics]과(와) Audience Manager 통합의 주요 이점은 다음과 같습니다.

+ **향상된 세그멘테이션**: 마케팅 캠페인에서 정밀하고 개인화된 대상 세그먼트를 위해 Adobe [!DNL Analytics]과(와) Audience Manager 데이터를 결합합니다.
+ **통합 고객 프로필**: 데이터 소스를 통합하여 상호 작용과 동작을 이해하고 포괄적인 고객 프로필을 만듭니다.
+ **광고 효율성 향상**: Adobe [!DNL Analytics] 및 Audience Manager 통합의 데이터 기반 타깃팅으로 광고를 최적화합니다.
+ **데이터 기반 결정**: 자세한 인사이트, [!DNL Analytics] Adobe 및 Audience Manager 데이터 병합을 통해 선택 사항을 알립니다.
+ **개인화된 경험**: 콘텐츠 및 오퍼를 맞춤화하여 두 플랫폼 모두 사용하여 터치포인트 간에 고객 상호 작용을 강화합니다.

전반적으로 이 통합은 중요한 데이터와 대상 통찰력을 하나로 모읍니다. 이를 통해 기업은 고객의 선호도와 행동을 더 깊이 이해하면서 타겟팅되고 관련성이 높은 마케팅 캠페인을 만들 수 있습니다.

## 일반적인 통합

<table>
    <thead>
        <tr>
            <th>Experience Cloud 애플리케이션</th>
            <th>를 사용하여 통합</th>
            <th>사용 시기</th>
            <th>일반적인 사용 사례</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] Audience Manager에게 데이터를 보내는 중</a>
            </td>
            <td>Adobe [!DNL Analytics] 태그 확장 또는 서버측 전달이 활성화된 AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>다른 Adobe Experience Cloud 대상, 사용자 기반 대상 또는 Audience Manager에서 지원하는 다른 장치 기반 및 사용자 지정 대상과 공유할 수 있는 세그먼트를 만들기 위해 Adobe [!DNL Analytics] 데이터를 Audience Manager에 보내려는 경우.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>[!DNL Analytics]에서 수집된 동작 특성을 포함하는 광고 플랫폼에 세그먼트를 공유합니다.</li>
                    <li>[!DNL Analytics] 데이터로 세그먼트를 보강하여 온사이트 타겟팅에 사용할 고부가가치의 크로스 채널 세그먼트를 만드십시오.</li>
                    <li>소셜 미디어 플랫폼에서 사용할 해시된 식별자(예: 이메일)를 키로 사용하는 세그먼트에 대한 [!DNL Analytics] 데이터의 계층입니다.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager이 데이터를 다시 [!DNL Analytics]</a>(으)로 전송 중
            </td>
            <td>Adobe [!DNL Analytics] 태그 확장 또는 서버측 전달이 활성화된 AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>대상 검색, 세분화 및 최적화를 알리기 위해 Audience Manager에서 [!DNL Analytics] (으)로 세그먼트를 공유하려는 경우.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>[!DNL Analytics] 보고서에 타사 공급자의 인구 통계학적 데이터를 포함하는 Audience Manager 세그먼트를 사용합니다.</li>
                    <li>[!DNL Analytics] 보고서에 광고 서버의 캠페인 데이터를 포함하는 Audience Manager 세그먼트를 사용합니다.</li>
                    <li>[!DNL Analytics] 보고서에 온보딩된 CRM 데이터를 포함하는 Audience Manager 세그먼트를 사용합니다.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
