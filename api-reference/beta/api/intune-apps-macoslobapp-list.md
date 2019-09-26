---
title: Listar macOSLobApps
description: Listar Propriedades e relações dos objetos macOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a55364c04d16a1f38dd054886568fbbe6d706b5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177665"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="ed5e4-103">Listar macOSLobApps</span><span class="sxs-lookup"><span data-stu-id="ed5e4-103">List macOSLobApps</span></span>

> <span data-ttu-id="ed5e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed5e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed5e4-106">Listar Propriedades e relações dos objetos [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ed5e4-106">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed5e4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed5e4-107">Prerequisites</span></span>
<span data-ttu-id="ed5e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed5e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed5e4-110">Permission type</span></span>|<span data-ttu-id="ed5e4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed5e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed5e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed5e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed5e4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed5e4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ed5e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed5e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed5e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-115">Not supported.</span></span>|
|<span data-ttu-id="ed5e4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed5e4-116">Application</span></span>|<span data-ttu-id="ed5e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed5e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed5e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed5e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ed5e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5e4-119">Request headers</span></span>
|<span data-ttu-id="ed5e4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed5e4-120">Header</span></span>|<span data-ttu-id="ed5e4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed5e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed5e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed5e4-122">Authorization</span></span>|<span data-ttu-id="ed5e4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed5e4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed5e4-124">Accept</span></span>|<span data-ttu-id="ed5e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed5e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5e4-126">Request body</span></span>
<span data-ttu-id="ed5e4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5e4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5e4-128">Response</span></span>
<span data-ttu-id="ed5e4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-129">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed5e4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed5e4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed5e4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5e4-131">Request</span></span>
<span data-ttu-id="ed5e4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ed5e4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5e4-133">Response</span></span>
<span data-ttu-id="ed5e4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed5e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2049

{
  "value": [
    {
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
  ]
}
```




