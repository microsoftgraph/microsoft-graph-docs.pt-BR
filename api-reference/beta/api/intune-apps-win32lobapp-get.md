---
title: Obter win32LobApp
description: Ler propriedades e relações do objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2895df0b881a5a52e6ddbcc6681f1d0b6c7189d7
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671321"
---
# <a name="get-win32lobapp"></a>Obter win32LobApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ler propriedades e relações do objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
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
Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3904

{
  "value": {
    "@odata.type": "#microsoft.graph.win32LobApp",
    "id": "9607b530-b530-9607-30b5-079630b50796",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "supersedingAppCount": 3,
    "supersededAppCount": 2,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "installCommandLine": "Install Command Line value",
    "uninstallCommandLine": "Uninstall Command Line value",
    "applicableArchitectures": "x86",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true,
      "v10_1909": true,
      "v10_2004": true,
      "v10_2H20": true,
      "v10_21H1": true
    },
    "minimumFreeDiskSpaceInMB": 8,
    "minimumMemoryInMB": 1,
    "minimumNumberOfProcessors": 9,
    "minimumCpuSpeedInMHz": 4,
    "detectionRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "detectionType": "exists",
        "operator": "equal",
        "detectionValue": "Detection Value value"
      }
    ],
    "requirementRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
        "operator": "equal",
        "detectionValue": "Detection Value value",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "detectionType": "exists"
      }
    ],
    "rules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
        "ruleType": "requirement",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "operationType": "exists",
        "operator": "equal",
        "comparisonValue": "Comparison Value value"
      }
    ],
    "installExperience": {
      "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
      "runAsAccount": "user",
      "deviceRestartBehavior": "allow"
    },
    "returnCodes": [
      {
        "@odata.type": "microsoft.graph.win32LobAppReturnCode",
        "returnCode": 10,
        "type": "success"
      }
    ],
    "msiInformation": {
      "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "upgradeCode": "Upgrade Code value",
      "requiresReboot": true,
      "packageType": "perUser",
      "productName": "Product Name value",
      "publisher": "Publisher value"
    },
    "setupFilePath": "Setup File Path value",
    "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
    "displayVersion": "Display Version value",
    "allowAvailableUninstall": true
  }
}
```




