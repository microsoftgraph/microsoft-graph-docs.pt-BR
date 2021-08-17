---
title: Atualizar userExperienceAnalyticsDeviceStartupHistory
description: Atualize as propriedades de um objeto userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efb2149bce5b3950f62a780ca1c8aedd3ce938e0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58261397"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a>Atualizar userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

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
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do histórico de inicialização do dispositivo de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A ID do dispositivo de análise de experiência do usuário.|
|startTime|DateTimeOffset|A hora de inicialização do dispositivo de análise de experiência do usuário.|
|coreBootTimeInMs|Int32|O tempo de inicialização principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyBootTimeInMs|Int32|Análise de experiência do usuário Tempo de inicialização da política de grupo do dispositivo em milissegundos.|
|featureUpdateBootTimeInMs|Int32|O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.|
|totalBootTimeInMs|Int32|O tempo total de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyLoginTimeInMs|Int32|Análise de experiência do usuário Tempo de logon da política de grupo do dispositivo em milissegundos.|
|coreLoginTimeInMs|Int32|O tempo de logon principal do dispositivo de análise de experiência do usuário em milissegundos.|
|responsiveDesktopTimeInMs|Int32|A análise da experiência do usuário responde ao tempo da área de trabalho em milissegundos.|
|totalLoginTimeInMs|Int32|O tempo total de logon do dispositivo de análise de experiência do usuário em milissegundos.|
|isFirstLogin|Boolean|O primeiro logon do dispositivo de análise de experiência do usuário.|
|isFeatureUpdate|Boolean|O registro de inicialização do dispositivo de análise de experiência do usuário é uma atualização de recurso.|
|operatingSystemVersion|String|A versão do sistema operacional do registro de inicialização do dispositivo de análise de experiência do usuário.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Categoria de reinicialização do sistema operacional. Os valores possíveis são: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|Cadeia de caracteres|Código de parada de reinicialização do sistema operacional. Isso mostra o código de verificação de bugs que pode ser usado para procurar o motivo da tela azul.|
|restartFaultBucket|Cadeia de caracteres|Bucket de falha de reinicialização do sistema operacional. O bucket de falhas é usado para encontrar informações adicionais sobre uma falha no sistema.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```




