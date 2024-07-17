---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# Adobe [!DNL Analytics]을(를) 실시간 고객 데이터 [!DNL Platform]과(와) 통합

{{analytics-description}}

{{real-time-cdp-description}}

Adobe [!DNL Analytics]을(를) Adobe 실시간 고객 데이터 [!DNL Platform](Real-Time CDP)와 통합하면 고객 경험과 마케팅 노력을 향상시키려는 비즈니스에 여러 가지 이점을 제공할 수 있습니다. 주요 이점은 다음과 같습니다.

+ **향상된 대상 타깃팅 및 개인화**: 장치 및 채널에 대한 정확한 마케팅, 최적화된 참여를 위한 맞춤 메시지.
+ **향상된 랜딩 페이지 최적화**: 장치 및 동작을 기반으로 맞춤화된 경험으로 사용자 만족도 및 전환을 개선했습니다.
+ **원활한 대상 활성화**: 선호하는 채널을 통해 효과적으로 타겟팅하고 관련 메시지를 게재하기 위해 고객 프로필을 활용하십시오.

Adobe [!DNL Analytics]과(와) Real-Time CDP을(를) 결합함으로써 기업은 마케팅 노력을 한 단계 더 발전시켜 개인화된 경험을 제공하고, 고객 참여를 높이고, 다양한 디지털 접점에서 전환을 최적화할 수 있습니다.

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
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] 원본 커넥터</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>[!DNL Analytics] Adobe을 이미 구현했으며 이 데이터를 [!DNL Platform] 경험에 가장 빠르게 수집하여 실시간 고객 프로필에서 사용하려는 고객에게 권장되는 방법입니다.</li>
                <li>실시간 고객 프로필에 대한 데이터 가용성이 데이터 수집 시간으로부터 2~30분 사이에 있을 수 있고 데이터 레이크에 대한 가용성은 최대 90분입니다.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>사용자 인터페이스가 시작한 간편한 워크플로우.</li>
                <li>사용자 인터페이스를 매핑하여 [!DNL Analytics] Prop 및 eVar를 새 XDM 필드에 복사합니다.</li>
                <li>실시간 고객 프로필 및 고객 여정 [!DNL Analytics]에서 가치를 얻는 가장 빠른 방법입니다.</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>새로운 [!DNL Analytics] 구현에 대한 권장 접근 방식 또는 장기적인 전략을 구현하려는 경우.</li>
                <li>AEP Web SDK, AEP Mobile SDK 또는 Edge Network 서버 API를 사용하여 장치에서 Experience [!DNL Platform](으)로 직접 데이터를 보냅니다.</li>
                <li>동일 및 다음 페이지 개인화 사용 사례를 지원하기 위해 실시간 고객 프로필에 [!DNL Analytics] 데이터 가용성이 필요한 신규 고객 또는 기존 고객.</li>
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
