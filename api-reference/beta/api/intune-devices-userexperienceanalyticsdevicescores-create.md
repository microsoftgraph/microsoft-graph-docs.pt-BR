---
title: Criar userExperienceAnalyticsDeviceScores
description: Crie um novo objeto userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60c16f45f80fc2d51c81496bcf1b0ad8af53ac24
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857901"
---
# <a name="create-userexperienceanalyticsdevicescores"></a>Criar userExperienceAnalyticsDeviceScores

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .

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
POST /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsDeviceScores.

A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsDeviceScores.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo de pontuações do dispositivo de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo de análise da experiência do usuário.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|endpointAnalyticsScore|Duplo|A pontuação do dispositivo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|appReliabilityScore|Duplo|A pontuação de confiabilidade do aplicativo de dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|workFromAnywhereScore|Duplo|A pontuação do dispositivo de análise de experiência do usuário funciona em qualquer lugar. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|batteryHealthScore|Duplo|A pontuação de integridade da bateria do dispositivo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade do dispositivo de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
Content-type: application/json
Content-length: 427

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 476

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```




