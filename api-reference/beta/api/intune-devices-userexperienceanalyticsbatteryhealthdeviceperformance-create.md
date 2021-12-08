---
title: Criar userExperienceAnalyticsBatteryHealthDevicePerformance
description: Crie um novo objeto userExperienceAnalyticsBatteryHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ae7ad86c4beb0dc221daef729cb6314944d56f0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343256"
---
# <a name="create-userexperienceanalyticsbatteryhealthdeviceperformance"></a>Criar userExperienceAnalyticsBatteryHealthDevicePerformance

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsBatteryHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)

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
POST /deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsBatteryHealthDevicePerformance.

A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsBatteryHealthDevicePerformance.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do dispositivo de saúde da bateria de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo, Intune DeviceID.|
|deviceName|String|Nome amigável do dispositivo.|
|modelo|String|O nome do modelo do dispositivo.|
|maxCapacityPercentage|Int32|Taxa de capacidade atual e capacidade de design da bateria com a menor capacidade. Unidade em porcentagem e valores variam de 0 a 100. Valores válidos -2147483648 para 2147483647|
|estimatedRuntimeInMinutes|Int32|O tempo de execução estimado do dispositivo quando a bateria é totalmente carregada. Unidade em minutos. Valores válidos -2147483648 para 2147483647|
|batteryAgeInDays|Int32|Idade estimada da bateria. Unidade em dias. Valores válidos -2147483648 para 2147483647|
|deviceBatteryHealthScore|Int32|Uma média ponderada da pontuação máxima de capacidade de um dispositivo e da pontuação da estimativa do tempo de execução. Os valores variam de 0 a 100. Valores válidos -2147483648 para 2147483647|
|healthStatus|String|O status geral da bateria do dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance
Content-type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 411

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "c8b9e0fd-e0fd-c8b9-fde0-b9c8fde0b9c8",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```




