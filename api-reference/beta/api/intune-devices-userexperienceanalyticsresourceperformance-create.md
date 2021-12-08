---
title: Criar userExperienceAnalyticsResourcePerformance
description: Crie um novo objeto userExperienceAnalyticsResourcePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd524b6fa70f59d21239e57238dbf58680d9c884
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334694"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a>Criar userExperienceAnalyticsResourcePerformance

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsResourcePerformance.

A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsResourcePerformance.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da entidade de desempenho do recurso de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceName|String|O nome do dispositivo.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|deviceCount|Int64|Contagem resumida de dispositivos da análise da experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|cpuSpikeTimePercentage|Duplo|Tempo de pico da CPU em porcentagem. Valores válidos de 0 a 100|
|ramSpikeTimePercentage|Duplo|Tempo de pico de RAM em porcentagem. Valores válidos de 0 a 100|
|cpuSpikeTimeScore|Int32|A pontuação de tempo de pico da CPU do dispositivo de análise de experiência do usuário. Valores válidos de 0 a 100|
|cpuSpikeTimePercentageThreshold|Duplo|Limite de cpuSpikeTimeScore. Valores válidos de 0 a 100|
|ramSpikeTimeScore|Int32|A pontuação do tempo de pico de RAM do dispositivo de análise de experiência do usuário. Valores válidos de 0 a 100|
|ramSpikeTimePercentageThreshold|Duplo|Limite de ramSpikeTimeScore. Valores válidos de 0 a 100|
|deviceResourcePerformanceScore|Int32|Pontuação de desempenho de recursos de um dispositivo específico. Valores válidos de 0 a 100|
|averageSpikeTimeScore|Int32|AverageSpikeTimeScore de um dispositivo ou um tipo de modelo. Valores válidos de 0 a 100|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14,
  "averageSpikeTimeScore": 5
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 633

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14,
  "averageSpikeTimeScore": 5
}
```




