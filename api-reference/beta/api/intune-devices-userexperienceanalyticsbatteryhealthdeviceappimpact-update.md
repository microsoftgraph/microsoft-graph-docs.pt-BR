---
title: Atualizar userExperienceAnalyticsBatteryHealthDeviceAppImpact
description: Atualize as propriedades de um objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a761791f969c66f966f6c0c9104e0068fbed2ae
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334428"
---
# <a name="update-userexperienceanalyticsbatteryhealthdeviceappimpact"></a>Atualizar userExperienceAnalyticsBatteryHealthDeviceAppImpact

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthDeviceAppImpact/{userExperienceAnalyticsBatteryHealthDeviceAppImpactId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o usuárioExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de impacto do aplicativo do dispositivo de bateria de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo, id do dispositivo Intune DeviceID ou SCCM.|
|appName|Cadeia de caracteres|Nome do aplicativo. Por exemplo: oltk.exe|
|appDisplayName|String|Nome de exibição amigável para o aplicativo. Por exemplo: Outlook|
|appPublisher|String|Editor de aplicativos. Por exemplo: Microsoft Corporation|
|isForegroundApp|Booliano|true se o usuário teve interação ativa com o aplicativo.|
|batteryUsagePercentage|Duplo|A porcentagem da energia total da bateria usada por esse aplicativo quando o dispositivo não foi conectado à energia ac, por mais de 14 dias. Unidade em porcentagem. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDeviceAppImpact/{userExperienceAnalyticsBatteryHealthDeviceAppImpactId}
Content-type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "deviceId": "Device Id value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 373

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "id": "30a55e18-5e18-30a5-185e-a530185ea530",
  "deviceId": "Device Id value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```




