---
title: Listar win32LobApps
description: Listar Propriedades e relações dos objetos win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe8a716b132fad4cf4750a5f42c957105819d43a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450584"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="3b8e7-103">Listar win32LobApps</span><span class="sxs-lookup"><span data-stu-id="3b8e7-103">List win32LobApps</span></span>

<span data-ttu-id="3b8e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b8e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b8e7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b8e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b8e7-107">Listar Propriedades e relações dos objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3b8e7-107">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b8e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b8e7-108">Prerequisites</span></span>
<span data-ttu-id="3b8e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b8e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b8e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b8e7-111">Permission type</span></span>|<span data-ttu-id="3b8e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b8e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b8e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b8e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b8e7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b8e7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3b8e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b8e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b8e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-116">Not supported.</span></span>|
|<span data-ttu-id="3b8e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b8e7-117">Application</span></span>|<span data-ttu-id="3b8e7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b8e7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b8e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b8e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3b8e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8e7-120">Request headers</span></span>
|<span data-ttu-id="3b8e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b8e7-121">Header</span></span>|<span data-ttu-id="3b8e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b8e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b8e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b8e7-123">Authorization</span></span>|<span data-ttu-id="3b8e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b8e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b8e7-125">Accept</span></span>|<span data-ttu-id="3b8e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b8e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b8e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8e7-127">Request body</span></span>
<span data-ttu-id="3b8e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b8e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b8e7-129">Response</span></span>
<span data-ttu-id="3b8e7-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-130">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b8e7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b8e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b8e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8e7-132">Request</span></span>
<span data-ttu-id="3b8e7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="3b8e7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b8e7-134">Response</span></span>
<span data-ttu-id="3b8e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b8e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3442

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
      "setupFilePath": "Setup File Path value",
      "installLanguage": "Install Language value"
    }
  ]
}
```





