---
title: Obter macOSLobApp
description: Leia as propriedades e as relações do objeto macOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb73eea7935fc74ed0a12d6b3605e289f8e18e11
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39919560"
---
# <a name="get-macoslobapp"></a><span data-ttu-id="50d7e-103">Obter macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="50d7e-103">Get macOSLobApp</span></span>

> <span data-ttu-id="50d7e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50d7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50d7e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50d7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50d7e-106">Leia as propriedades e as relações do objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="50d7e-106">Read properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d7e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50d7e-107">Prerequisites</span></span>
<span data-ttu-id="50d7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50d7e-110">Permission type</span></span>|<span data-ttu-id="50d7e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50d7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50d7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50d7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50d7e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50d7e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="50d7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50d7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50d7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50d7e-115">Not supported.</span></span>|
|<span data-ttu-id="50d7e-116">Application</span><span class="sxs-lookup"><span data-stu-id="50d7e-116">Application</span></span>|<span data-ttu-id="50d7e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50d7e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50d7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50d7e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50d7e-119">Optional query parameters</span></span>
<span data-ttu-id="50d7e-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50d7e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50d7e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50d7e-121">Request headers</span></span>
|<span data-ttu-id="50d7e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50d7e-122">Header</span></span>|<span data-ttu-id="50d7e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="50d7e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50d7e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="50d7e-124">Authorization</span></span>|<span data-ttu-id="50d7e-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50d7e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50d7e-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50d7e-126">Accept</span></span>|<span data-ttu-id="50d7e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50d7e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d7e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50d7e-128">Request body</span></span>
<span data-ttu-id="50d7e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50d7e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d7e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d7e-130">Response</span></span>
<span data-ttu-id="50d7e-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50d7e-131">If successful, this method returns a `200 OK` response code and [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d7e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50d7e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d7e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50d7e-133">Request</span></span>
<span data-ttu-id="50d7e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50d7e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="50d7e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d7e-135">Response</span></span>
<span data-ttu-id="50d7e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50d7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1921

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
    "ignoreVersionDetection": true
  }
}
```





