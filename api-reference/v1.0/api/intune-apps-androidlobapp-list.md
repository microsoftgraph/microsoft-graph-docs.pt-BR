---
title: Listar androidLobApps
description: Listar propriedades e relações dos objetos androidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f1b54791a67c85498a474b93ced0714b5bd20b9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358988"
---
# <a name="list-androidlobapps"></a><span data-ttu-id="70c8f-103">Listar androidLobApps</span><span class="sxs-lookup"><span data-stu-id="70c8f-103">List androidLobApps</span></span>

> <span data-ttu-id="70c8f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70c8f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c8f-105">Listar propriedades e relações dos objetos [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="70c8f-105">List properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70c8f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70c8f-106">Prerequisites</span></span>
<span data-ttu-id="70c8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c8f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70c8f-109">Permission type</span></span>|<span data-ttu-id="70c8f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70c8f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70c8f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70c8f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70c8f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c8f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70c8f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70c8f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70c8f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70c8f-114">Not supported.</span></span>|
|<span data-ttu-id="70c8f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70c8f-115">Application</span></span>|<span data-ttu-id="70c8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70c8f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70c8f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70c8f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="70c8f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70c8f-118">Request headers</span></span>
|<span data-ttu-id="70c8f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70c8f-119">Header</span></span>|<span data-ttu-id="70c8f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="70c8f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70c8f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="70c8f-121">Authorization</span></span>|<span data-ttu-id="70c8f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70c8f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70c8f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70c8f-123">Accept</span></span>|<span data-ttu-id="70c8f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70c8f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c8f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70c8f-125">Request body</span></span>
<span data-ttu-id="70c8f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70c8f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70c8f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="70c8f-127">Response</span></span>
<span data-ttu-id="70c8f-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70c8f-128">If successful, this method returns a `200 OK` response code and a collection of [androidLobApp](../resources/intune-apps-androidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c8f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70c8f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="70c8f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70c8f-130">Request</span></span>
<span data-ttu-id="70c8f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70c8f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="70c8f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="70c8f-132">Response</span></span>
<span data-ttu-id="70c8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70c8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidLobApp",
      "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "packageId": "Package Id value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value"
    }
  ]
}
```




