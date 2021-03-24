---
title: Obter macOSLobApp
description: Leia propriedades e relações do objeto macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 132f54fa56d1fbb7c8e184670d2e5294a0645ccd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143959"
---
# <a name="get-macoslobapp"></a><span data-ttu-id="c7a68-103">Obter macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="c7a68-103">Get macOSLobApp</span></span>

<span data-ttu-id="c7a68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7a68-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7a68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7a68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7a68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a68-107">Leia propriedades e relações do [objeto macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c7a68-107">Read properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7a68-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7a68-108">Prerequisites</span></span>
<span data-ttu-id="c7a68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7a68-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7a68-111">Permission type</span></span>|<span data-ttu-id="c7a68-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7a68-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7a68-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7a68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7a68-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a68-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7a68-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7a68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7a68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7a68-116">Not supported.</span></span>|
|<span data-ttu-id="c7a68-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7a68-117">Application</span></span>|<span data-ttu-id="c7a68-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a68-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7a68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7a68-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7a68-120">Optional query parameters</span></span>
<span data-ttu-id="c7a68-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a68-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7a68-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a68-122">Request headers</span></span>
|<span data-ttu-id="c7a68-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7a68-123">Header</span></span>|<span data-ttu-id="c7a68-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c7a68-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7a68-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7a68-125">Authorization</span></span>|<span data-ttu-id="c7a68-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a68-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7a68-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7a68-127">Accept</span></span>|<span data-ttu-id="c7a68-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7a68-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7a68-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a68-129">Request body</span></span>
<span data-ttu-id="c7a68-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7a68-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7a68-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a68-131">Response</span></span>
<span data-ttu-id="c7a68-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a68-132">If successful, this method returns a `200 OK` response code and [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7a68-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7a68-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7a68-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a68-134">Request</span></span>
<span data-ttu-id="c7a68-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a68-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="c7a68-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a68-136">Response</span></span>
<span data-ttu-id="c7a68-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7a68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2013

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSLobApp",
    "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
    "bundleId": "Bundle Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
      "v10_7": true,
      "v10_8": true,
      "v10_9": true,
      "v10_10": true,
      "v10_11": true,
      "v10_12": true,
      "v10_13": true,
      "v10_14": true,
      "v10_15": true
    },
    "buildNumber": "Build Number value",
    "versionNumber": "Version Number value",
    "childApps": [
      {
        "@odata.type": "microsoft.graph.macOSLobChildApp",
        "bundleId": "Bundle Id value",
        "buildNumber": "Build Number value",
        "versionNumber": "Version Number value"
      }
    ],
    "identityVersion": "Identity Version value",
    "md5HashChunkSize": 0,
    "md5Hash": [
      "Md5Hash value"
    ],
    "ignoreVersionDetection": true,
    "installAsManaged": true
  }
}
```




