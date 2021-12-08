---
title: Função userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2de62f3f75e3c378bfedfcfa481cc043f8f6ac80
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337809"
---
# <a name="userexperienceanalyticssummarizeworkfromanywheredevices-function"></a>Função userExperienceAnalyticsSummarizeWorkFromAnywhereDevices

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

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
GET /deviceManagement/userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, essa função retornará um código de resposta e um `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevicesSummary](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevicessummary.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1355

{
  "value": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
    "autopilotDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
      "devicesNotAutopilotRegistered": 13,
      "devicesWithoutAutopilotProfileAssigned": 6,
      "totalWindows10DevicesWithoutTenantAttached": 10
    },
    "cloudManagementDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
      "coManagedDeviceCount": 4,
      "intuneDeviceCount": 1,
      "tenantAttachDeviceCount": 7
    },
    "windows10DevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
      "unsupportedOSversionDeviceCount": 15
    },
    "cloudIdentityDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
      "deviceWithoutCloudIdentityCount": 15
    },
    "totalDevices": 12,
    "coManagedDevices": 0,
    "intuneDevices": 13,
    "tenantAttachDevices": 3,
    "windows10Devices": 0,
    "windows10DevicesWithoutTenantAttach": 3,
    "unsupportedOSversionDevices": 11,
    "devicesWithoutCloudIdentity": 11,
    "devicesNotAutopilotRegistered": 13,
    "devicesWithoutAutopilotProfileAssigned": 6
  }
}
```




