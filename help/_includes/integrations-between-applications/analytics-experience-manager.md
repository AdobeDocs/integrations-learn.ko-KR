---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 8%

---


# [!DNL Analytics] 및 Experience Manager 통합

{{analytics-description}}

{{experience-manager-description}}

통합 Adobe [!DNL Analytics] 그리고 Adobe Experience Manager은 다음을 포함한 몇 가지 이점을 제공합니다.

+ **정확한 세분화**: 병합 Adobe [!DNL Analytics] 캠페인의 개인화된 대상 세그먼트에 대한 &amp; Audience Manager.
+ **포괄적인 고객** 프로필: 데이터 소스를 통합하여 상호 작용 및 동작을 통합적으로 이해할 수 있습니다.
+ **최적화된 광고 타깃팅**: Adobe의 데이터 기반 타겟팅을 통해 광고 효과 향상 [!DNL Analytics] 및 Audience Manager.
+ **정보에 입각한 결정**: 병합된 Adobe의 자세한 인사이트 [!DNL Analytics] 더 나은 선택을 위한 &amp; Audience Manager 데이터.
+ **개인화된 경험**: 두 플랫폼의 기능을 모두 활용하여 터치포인트 간에 개인화된 콘텐츠 및 오퍼를 제공합니다.

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
            <td rowspan="2">[!DNL Analytics] AEM Sites 사용</a></td>
            <td><a href="https://experienceleague.adobe.com/docs/experience-manager-learn/sites/integrations/experience-platform/analytics-using-web-sdk.html" target="_blank" rel="noreferrer">경험 [!DNL Platform] Web SDK 태그 확장 또는 alloy.js</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Adobe에서 AEM 웹 분석 데이터에 대해 보고하려는 경우 [!DNL Analytics]를 참조하고 향후 다른 Experience Cloud 애플리케이션과 통합할 수 있습니다.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                  <li>웹 사이트 트래픽 추적.</li>
                  <li>마케팅 캠페인 모니터링</li>
                  <li>웹 사이트 성능 최적화.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="https://experienceleague.adobe.com/docs/experience-manager-learn/sites/integrations/analytics/collect-data-analytics.html" target="_blank" rel="noreferrer">Adobe [!DNL Analytics] 태그 확장 또는 AppMeasurement.js</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Adobe에서 AEM 웹 분석 데이터에 대해 보고하려는 경우 [!DNL Analytics], 및 은(는) 다른 Experience Cloud 애플리케이션에서 데이터를 사용할 계획이 없습니다</li>
                    <li>추적 가능한 웹 사이트 요소에 AEM 핵심 구성 요소를 사용하는 경우.</li>
                    <li>최소 구성 및 구현이 필요한 경우.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                  <li>웹 사이트 트래픽 추적.</li>
                  <li>마케팅 캠페인 모니터링</li>
                  <li>웹 사이트 성능 최적화.</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="https://experienceleague.adobe.com/docs/experience-manager-learn/cloud-service/forms/forms-and-analytics/introduction.html" target="_blank" rel="noreferrer">[!DNL Analytics] 및 Cloud Service으로 AEM Forms</a></td>
            <td>경험 [!DNL Platform] Web SDK 태그 확장</td>
            <td>
              <ul style="margin-top: 0;">
                <li>Adobe에서 디지털 양식 분석 데이터를 보고하려는 경우 [!DNL Analytics]를 참조하고 향후 다른 Experience Cloud 애플리케이션과 통합할 수 있습니다.</li>
              </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                  <li>양식 제출을 추적합니다.</li>
                  <li>양식 필드 오류 모니터링</li>
                  <li>제출된 양식 필드 값에 대해 보고합니다.</li>
                </ul>
            </td>
        </tr>
    </tbody>          
</table>
