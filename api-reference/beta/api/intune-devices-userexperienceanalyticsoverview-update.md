---
title: Atualizar userExperienceAnalyticsOverview
description: Atualize as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e48c464c19e17873b7dee59f0e3e5a54cc827adf
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58261198"
---
# <a name="update-userexperienceanalyticsoverview"></a>Atualizar userExperienceAnalyticsOverview

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da visão geral da análise de experiência do usuário.|
|overallScore|Int32|A pontuação geral da análise de experiência do usuário.|
|deviceBootPerformanceOverallScore|Int32|A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.|
|bestPracticesOverallScore|Int32|A pontuação geral das práticas recomendadas da análise da experiência do usuário.|
|workFromAnywhereOverallScore|Int32|A pontuação geral da análise de experiência do usuário Work From Anywhere.|
|appHealthOverallScore|Int32|A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.|
|resourcePerformanceOverallScore|Int32|A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.|
|insights|[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|As percepções de análise de experiência do usuário.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da visão geral da análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices". Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'WorkFromAnywhere'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices". Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 1005

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```




