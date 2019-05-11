---
title: Obter win32LobApp
description: Leia as propriedades e as relações do objeto win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 331ca0eafe11f1a5f0a0de3b9cda4f9082af0082
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934821"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="cc364-103">Obter win32LobApp</span><span class="sxs-lookup"><span data-stu-id="cc364-103">Get win32LobApp</span></span>

> <span data-ttu-id="cc364-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc364-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc364-106">Leia as propriedades e as relações do objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="cc364-106">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc364-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc364-107">Prerequisites</span></span>
<span data-ttu-id="cc364-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc364-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc364-110">Permission type</span></span>|<span data-ttu-id="cc364-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc364-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc364-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc364-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc364-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc364-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cc364-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc364-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc364-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc364-115">Not supported.</span></span>|
|<span data-ttu-id="cc364-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc364-116">Application</span></span>|<span data-ttu-id="cc364-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc364-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc364-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc364-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc364-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc364-119">Optional query parameters</span></span>
<span data-ttu-id="cc364-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc364-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc364-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc364-121">Request headers</span></span>
|<span data-ttu-id="cc364-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc364-122">Header</span></span>|<span data-ttu-id="cc364-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cc364-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc364-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc364-124">Authorization</span></span>|<span data-ttu-id="cc364-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc364-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc364-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc364-126">Accept</span></span>|<span data-ttu-id="cc364-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cc364-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc364-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc364-128">Request body</span></span>
<span data-ttu-id="cc364-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc364-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc364-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc364-130">Response</span></span>
<span data-ttu-id="cc364-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc364-131">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc364-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc364-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc364-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc364-133">Request</span></span>
<span data-ttu-id="cc364-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc364-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="cc364-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc364-135">Response</span></span>
<span data-ttu-id="cc364-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc364-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3101

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
      "v10_1803": true
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
      "runAsAccount": "user"
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
}
```




