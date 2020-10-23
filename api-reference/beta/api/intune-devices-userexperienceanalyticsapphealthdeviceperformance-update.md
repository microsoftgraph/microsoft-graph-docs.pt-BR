---
title: Atualizar userExperienceAnalyticsAppHealthDevicePerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2408ad8564411c58c5d65eeb41fb6ce82a491aec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693189"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a>Atualizar userExperienceAnalyticsAppHealthDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.|
|deviceModel|Cadeia de caracteres|O nome do modelo do dispositivo.|
|deviceManufacturer|String|O nome do fabricante do dispositivo.|
|appCrashCount|Int32|O número de falhas do aplicativo para o dispositivo. Valores válidos-2147483648 a 2147483647|
|crashedAppCount|Int32|O número de falhas de aplicativos distintos para o dispositivo. Valores válidos-2147483648 a 2147483647|
|appHangCount|Int32|O número de bloqueios de aplicativo para o dispositivo. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo médio de falha para o dispositivo em minutos. Valores válidos-2147483648 a 2147483647|
|deviceAppHealthScore|Duplo|A pontuação de integridade do aplicativo do dispositivo. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|deviceAppHealthStatus|String|O status de integridade geral do aplicativo do dispositivo.|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|deviceDisplayName|Cadeia de caracteres|O nome do dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```





