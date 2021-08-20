---
title: Atualizar userExperienceAnalyticsDevicePerformance
description: Atualize as propriedades de um objeto userExperienceAnalyticsDevicePerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 942d20ac2b8b8a335da57103e516d0a5520b5bce
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264868"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a>Atualizar userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)

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
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsDevicePerformance.](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo de análise de experiência do usuário.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|O tipo de disco do dispositivo de análise de experiência do usuário. Os valores possíveis são: `unkown`, `hdd`, `ssd`.|
|operatingSystemVersion|String|A versão do sistema operacional do dispositivo de análise de experiência do usuário.|
|bootScore|Int32|A pontuação de inicialização do dispositivo de análise de experiência do usuário.|
|coreBootTimeInMs|Int32|O tempo de inicialização principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyBootTimeInMs|Int32|O tempo de inicialização da política de grupo de dispositivos de análise de experiência do usuário em milissegundos.|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde do dispositivo de análise de experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32|A pontuação de logon do dispositivo de análise de experiência do usuário.|
|coreLoginTimeInMs|Int32|O tempo de logon principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyLoginTimeInMs|Int32|O tempo de logon da política de grupo de dispositivos de análise de experiência do usuário em milissegundos.|
|deviceCount|Int64|Contagem resumida de dispositivos da análise da experiência do usuário.|
|responsiveDesktopTimeInMs|Int32|A análise da experiência do usuário responde ao tempo da área de trabalho em milissegundos.|
|blueScreenCount|Int32|Número de telas azuis nos últimos 14 dias. Valores válidos de 0 a 9999999|
|restartCount|Int32|Número de reinicializações nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageBlueScreens|Duplo|Número médio (médio) de Telas Azuis por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageRestarts|Duplo|Número médio (médio) de Reinicializações por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 733

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "852ae826-e826-852a-26e8-2a8526e82a85",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0,
  "startupPerformanceScore": 7.666666666666667
}
```




