---
title: Obter win32LobApp
description: Leia propriedades e relações do objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab7f1add39df14c6cd01ae66f10300607228dad8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142881"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="d17ca-103">Obter win32LobApp</span><span class="sxs-lookup"><span data-stu-id="d17ca-103">Get win32LobApp</span></span>

<span data-ttu-id="d17ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d17ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d17ca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d17ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d17ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d17ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d17ca-107">Leia propriedades e relações do [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d17ca-107">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d17ca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d17ca-108">Prerequisites</span></span>
<span data-ttu-id="d17ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d17ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d17ca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d17ca-111">Permission type</span></span>|<span data-ttu-id="d17ca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d17ca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d17ca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d17ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d17ca-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17ca-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d17ca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d17ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d17ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d17ca-116">Not supported.</span></span>|
|<span data-ttu-id="d17ca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d17ca-117">Application</span></span>|<span data-ttu-id="d17ca-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17ca-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d17ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d17ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d17ca-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d17ca-120">Optional query parameters</span></span>
<span data-ttu-id="d17ca-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d17ca-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d17ca-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d17ca-122">Request headers</span></span>
|<span data-ttu-id="d17ca-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d17ca-123">Header</span></span>|<span data-ttu-id="d17ca-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d17ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d17ca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d17ca-125">Authorization</span></span>|<span data-ttu-id="d17ca-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d17ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d17ca-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d17ca-127">Accept</span></span>|<span data-ttu-id="d17ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d17ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d17ca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d17ca-129">Request body</span></span>
<span data-ttu-id="d17ca-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d17ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d17ca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d17ca-131">Response</span></span>
<span data-ttu-id="d17ca-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d17ca-132">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d17ca-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d17ca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d17ca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d17ca-134">Request</span></span>
<span data-ttu-id="d17ca-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d17ca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d17ca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d17ca-136">Response</span></span>
<span data-ttu-id="d17ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d17ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3816

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
      "v10_2004": true
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
    "displayVersion": "Display Version value"
  }
}
```




