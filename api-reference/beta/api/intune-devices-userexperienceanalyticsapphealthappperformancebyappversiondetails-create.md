---
title: Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails
description: Crie um novo objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bf23c97785e7d9981c08c5ca47a9189da1558f4
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342367"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversiondetails"></a>Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md)

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
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDetails
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.

A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.|
|deviceCountWithCrashes|Int32|O número total de dispositivos que relataram falhas de um ou mais aplicativos para este aplicativo e versão. Valores válidos -2147483648 para 2147483647|
|isMostUsedVersion|Booliano|É a versão do aplicativo a versão mais usada para esse aplicativo.|
|isLatestUsedVersion|Boolean|É a versão do aplicativo a versão mais recente para esse aplicativo que está em uso.|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|String|O nome amigável do aplicativo.|
|appPublisher|String|O editor do aplicativo.|
|appVersion|String|A versão do aplicativo.|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos -2147483648 para 2147483647|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondetails.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDetails
Content-type: application/json
Content-length: 384

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails",
  "deviceCountWithCrashes": 6,
  "isMostUsedVersion": true,
  "isLatestUsedVersion": true,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDetails",
  "id": "1505e3e6-e3e6-1505-e6e3-0515e6e30515",
  "deviceCountWithCrashes": 6,
  "isMostUsedVersion": true,
  "isLatestUsedVersion": true,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```




