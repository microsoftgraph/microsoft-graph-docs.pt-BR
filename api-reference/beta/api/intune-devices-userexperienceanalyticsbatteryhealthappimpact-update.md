---
title: Atualizar userExperienceAnalyticsBatteryHealthAppImpact
description: Atualize as propriedades de um objeto userExperienceAnalyticsBatteryHealthAppImpact.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ecb7dc37f81804c04851c54eb9e7d3d07add883
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339931"
---
# <a name="update-userexperienceanalyticsbatteryhealthappimpact"></a>Atualizar userExperienceAnalyticsBatteryHealthAppImpact

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthAppImpact/{userExperienceAnalyticsBatteryHealthAppImpactId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de impacto do aplicativo de bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para usar esse aplicativo em um período de 14 dias. Valores válidos -2147483648 para 2147483647|
|appName|Cadeia de caracteres|Nome do aplicativo. Por exemplo: oltk.exe|
|appDisplayName|String|Nome de exibição amigável para o aplicativo. Por exemplo: Outlook|
|appPublisher|String|Editor de aplicativos. Por exemplo: Microsoft Corporation|
|isForegroundApp|Booliano|true se o usuário teve interação ativa com o aplicativo.|
|batteryUsagePercentage|Duplo|A porcentagem da energia total da bateria usada por esse aplicativo quando o dispositivo não estava conectado à energia ac, mais de 14 dias computado em todos os dispositivos no locatário. Unidade em porcentagem. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthAppImpact/{userExperienceAnalyticsBatteryHealthAppImpactId}
Content-type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "activeDevices": 13,
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
Content-Length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "id": "d2a9c89a-c89a-d2a9-9ac8-a9d29ac8a9d2",
  "activeDevices": 13,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```




