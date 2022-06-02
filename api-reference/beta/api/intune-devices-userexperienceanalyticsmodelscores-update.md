---
title: Atualizar userExperienceAnalyticsModelScores
description: Atualize as propriedades de um objeto userExperienceAnalyticsModelScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7964a0ea56aeffb5f166cf3076d9a09aa39092ed
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857873"
---
# <a name="update-userexperienceanalyticsmodelscores"></a>Atualizar userExperienceAnalyticsModelScores

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de pontuações do modelo de análise de experiência do usuário.|
|modelo|String|Um identificador exclusivo das pontuações do modelo de análise de experiência do usuário: modelo de dispositivo.|
|fabricante|String|Um identificador exclusivo das pontuações do modelo de análise de experiência do usuário: fabricante do dispositivo.|
|modelDeviceCount|Int64|A contagem de dispositivos do modelo de análise de experiência do usuário. Valores válidos -9.22337203685478E+18 a 9.22337203685478E+18|
|endpointAnalyticsScore|Duplo|A pontuação do modelo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|appReliabilityScore|Duplo|A pontuação de confiabilidade do aplicativo de modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|workFromAnywhereScore|Duplo|A pontuação do modelo de análise de experiência do usuário funciona em qualquer lugar. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|batteryHealthScore|Duplo|A pontuação de integridade da bateria do modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade do modelo de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "f2c0f69c-f69c-f2c0-9cf6-c0f29cf6c0f2",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```




