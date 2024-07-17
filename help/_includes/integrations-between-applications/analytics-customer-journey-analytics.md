---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Adobe [!DNL Analytics]을(를) 고객 여정 [!DNL Analytics]과(와) 통합

{{analytics-description}}

{{customer-journey-analytics-description}}

[!DNL Analytics] Adobe을 [!DNL Analytics] 고객 여정과 통합하면 다음과 같은 주요 이점이 있습니다.

+ 고객 행동 및 환경 설정에 대한 **종합적인 통찰력**.
+ 전체적인 보기를 위해 **원활한 크로스 채널 추적**.
+ 정확한 분석을 위해 **통합 데이터 및 보고**.
+ **향상된 개인화** 및 향상된 고객 참여
+ 애자일 의사 결정을 위한 **실시간 데이터 인사이트**.

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
            <td rowspan="2">[!DNL Analytics] 및 고객 여정 [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] 원본 커넥터</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>[!DNL Analytics] Adobe을 이미 구현했으며 고객 여정 [!DNL Analytics]에서 사용할 수 있도록 이 데이터를 [!DNL Platform] 경험에 수집하는 가장 빠른 방법을 원하는 고객에게 권장되는 방법입니다.</li>
                    <li>고객 프로필에 대한 데이터 가용성이 데이터 수집 시점부터 2~30분일 수 있고 데이터 레이크에 대한 가용성은 최대 90분입니다.</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">경험 [!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>새로운 [!DNL Analytics] 구현에 대한 권장 접근 방식 또는 장기적인 전략을 구현하려는 경우.</li>
                    <li>AEP Web SDK, AEP Mobile SDK 또는 Edge Network 서버 API를 사용하여 장치에서 Experience [!DNL Platform](으)로 직접 데이터를 보냅니다.</li>
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
    </tbody>          
</table>
