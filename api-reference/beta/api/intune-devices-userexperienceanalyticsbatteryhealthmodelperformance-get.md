---
title: Obter userExperienceAnalyticsBatteryHealthModelPerformance
description: Ler propriedades e relações do objeto userExperienceAnalyticsBatteryHealthModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e459ff5531c1a2c86eccc2495b5ecc118515c68
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857782"
---
# <a name="get-userexperienceanalyticsbatteryhealthmodelperformance"></a>Obter userExperienceAnalyticsBatteryHealthModelPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ler propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance/{userExperienceAnalyticsBatteryHealthModelPerformanceId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este `200 OK` método retorna um código de resposta e o objeto [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance/{userExperienceAnalyticsBatteryHealthModelPerformanceId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
    "id": "0850afa4-afa4-0850-a4af-5008a4af5008",
    "activeDevices": 13,
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "averageMaxCapacityPercentage": 12,
    "averageEstimatedRuntimeInMinutes": 0,
    "averageBatteryAgeInDays": 7,
    "modelBatteryHealthScore": 7
  }
}
```




