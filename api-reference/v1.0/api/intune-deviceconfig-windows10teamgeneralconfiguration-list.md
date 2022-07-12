---
title: Listar windows10TeamGeneralConfigurations
description: Listar propriedades e relações dos objetos windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9c7cacb81efd4a43f8ef82c5e5fcde275ac0dc3e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734036"
---
# <a name="list-windows10teamgeneralconfigurations"></a>Listar windows10TeamGeneralConfigurations

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Listar propriedades e relações dos objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
      "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "azureOperationalInsightsBlockTelemetry": true,
      "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
      "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
      "connectAppBlockAutoLaunch": true,
      "maintenanceWindowBlocked": true,
      "maintenanceWindowDurationInHours": 0,
      "maintenanceWindowStartTime": "11:59:09.3130000",
      "miracastChannel": "one",
      "miracastBlocked": true,
      "miracastRequirePin": true,
      "settingsBlockMyMeetingsAndFiles": true,
      "settingsBlockSessionResume": true,
      "settingsBlockSigninSuggestions": true,
      "settingsDefaultVolume": 5,
      "settingsScreenTimeoutInMinutes": 14,
      "settingsSessionTimeoutInMinutes": 15,
      "settingsSleepTimeoutInMinutes": 13,
      "welcomeScreenBlockAutomaticWakeUp": true,
      "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
      "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
    }
  ]
}
```





