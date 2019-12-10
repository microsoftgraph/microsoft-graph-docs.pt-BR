---
title: Listar win32LobApps
description: Listar Propriedades e relações dos objetos win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1ba6d23b5f712d99f6d6d080cd024a14c2e56aa
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933927"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="63123-103">Listar win32LobApps</span><span class="sxs-lookup"><span data-stu-id="63123-103">List win32LobApps</span></span>

> <span data-ttu-id="63123-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63123-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63123-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63123-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63123-106">Listar Propriedades e relações dos objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="63123-106">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63123-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63123-107">Prerequisites</span></span>
<span data-ttu-id="63123-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63123-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63123-110">Permission type</span></span>|<span data-ttu-id="63123-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63123-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63123-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63123-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63123-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63123-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63123-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63123-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63123-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63123-115">Not supported.</span></span>|
|<span data-ttu-id="63123-116">Application</span><span class="sxs-lookup"><span data-stu-id="63123-116">Application</span></span>|<span data-ttu-id="63123-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63123-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63123-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63123-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="63123-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63123-119">Request headers</span></span>
|<span data-ttu-id="63123-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63123-120">Header</span></span>|<span data-ttu-id="63123-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63123-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63123-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63123-122">Authorization</span></span>|<span data-ttu-id="63123-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63123-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63123-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63123-124">Accept</span></span>|<span data-ttu-id="63123-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63123-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63123-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63123-126">Request body</span></span>
<span data-ttu-id="63123-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63123-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63123-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="63123-128">Response</span></span>
<span data-ttu-id="63123-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63123-129">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63123-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63123-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="63123-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63123-131">Request</span></span>
<span data-ttu-id="63123-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63123-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="63123-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="63123-133">Response</span></span>
<span data-ttu-id="63123-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63123-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3390

{
  "value": [
    {
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
        "v10_1903": true
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
      "setupFilePath": "Setup File Path value"
    }
  ]
}
```





