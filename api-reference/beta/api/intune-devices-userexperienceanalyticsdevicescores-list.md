---
title: Listar userExperienceAnalyticsDeviceScoreses
description: Listar propriedades e relações dos objetos userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32800e58236080777544150344fb07d71e4766a4
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858230"
---
# <a name="list-userexperienceanalyticsdevicescoreses"></a>Listar userExperienceAnalyticsDeviceScoreses

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .

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
GET /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método `200 OK` retornará um código de resposta e uma coleção de [objetos userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "value": [
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
  ]
}
```




