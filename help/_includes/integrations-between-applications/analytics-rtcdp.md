---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 1%

---


# 통합 Adobe [!DNL Analytics] 실시간 고객 데이터 포함 [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

통합 Adobe [!DNL Analytics] Adobe 실시간 고객 데이터 [!DNL Platform] (Real-Time CDP)는 고객 경험과 마케팅 노력을 향상시키고자 하는 비즈니스에 몇 가지 이점을 제공할 수 있습니다. 주요 이점은 다음과 같습니다.

+ **향상된 대상 타깃팅 및 개인화**: 장치 및 채널에 대한 정확한 마케팅, 최적화된 참여를 위한 맞춤 메시지.
+ **향상된 랜딩 페이지 최적화**: 장치 및 행동에 따라 맞춤 설정된 경험으로 사용자 만족도 및 전환을 향상시킵니다.
+ **원활한 대상 활성화**: 선호하는 채널을 통한 효과적인 타겟팅에 고객 프로필을 활용하여 관련 메시지를 전달할 수 있습니다.

Adobe 결합 [!DNL Analytics] 그리고 Real-Time CDP은 기업이 마케팅 노력을 한 단계 더 발전시켜 개인화된 경험을 제공하고, 고객 참여를 높이고, 다양한 디지털 접점에서 전환을 최적화할 수 있습니다.

<table>
    <thead>
        <tr>
            <th>Experience Cloud 애플리케이션</th>
            <th>를 사용하여 통합</th>
            <th>사용 시기</th>
            <th>일반적인 사용 사례</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] Real-Time CDP 사용</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] 소스 커넥터</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>이미 Adobe을 구현한 고객에 대한 권장 접근 방식 [!DNL Analytics], 그리고 이 데이터를 Experience에 수집하는 가장 빠른 방법이 필요합니다 [!DNL Platform] 실시간 고객 프로필에서 를 사용하도록 설정합니다.</li>
                <li>실시간 고객 프로필에 대한 데이터 가용성이 데이터 수집 시간으로부터 2~30분 사이에 있을 수 있고 데이터 레이크에 대한 가용성은 최대 90분입니다.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>사용자 인터페이스가 시작한 간편한 워크플로우.</li>
                <li>사용자 인터페이스를 복사하도록 매핑 [!DNL Analytics] 새 XDM 필드에 대한 prop 및 eVar.</li>
                <li>실시간 고객 프로필 및 고객 여정에서 가치를 얻는 가장 빠른 방법 [!DNL Analytics].</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>새로운 사용자를 위한 권장 접근 방식 [!DNL Analytics] 구현 또는 장기적인 전략을 구현하려는 경우.</li>
                <li>장치에서 경험으로 직접 데이터 전송 [!DNL Platform] aep 웹 SDK, AEP 모바일 SDK 또는 Edge Network Server API 사용.</li>
                <li>필요한 신규 또는 기존 고객 [!DNL Analytics] 실시간 고객 프로필에 대한 데이터 가용성을 확인하여 동일한 페이지 개인화 사용 사례를 지원합니다.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>사용 사례를 지원하기 위해 사용하기 위해 수집된 데이터에 대해 가장 높은 수준의 제어 기능을 제공합니다.</li>
                <li>클라이언트측 데이터는 XDM 필드에 쉽게 매핑됩니다.</li>
                <li>실시간 고객 프로필에서 데이터를 가장 빠르게 사용할 수 있습니다.</li>
            </ul>
        </td>
    </tr>            
</table>
