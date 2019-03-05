---
title: Listar windowsMobileMSIs
description: Listar propriedades e relações dos objetos windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9a81b53b3c715c09baf2d05d65ee6a0b2a7cd2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156333"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="12459-103">Listar windowsMobileMSIs</span><span class="sxs-lookup"><span data-stu-id="12459-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="12459-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12459-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12459-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12459-106">Listar propriedades e relações dos objetos [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="12459-106">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12459-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12459-107">Prerequisites</span></span>
<span data-ttu-id="12459-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="12459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12459-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12459-110">Permission type</span></span>|<span data-ttu-id="12459-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12459-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12459-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12459-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12459-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12459-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12459-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12459-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12459-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12459-115">Not supported.</span></span>|
|<span data-ttu-id="12459-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12459-116">Application</span></span>|<span data-ttu-id="12459-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12459-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12459-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12459-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="12459-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12459-119">Request headers</span></span>
|<span data-ttu-id="12459-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12459-120">Header</span></span>|<span data-ttu-id="12459-121">Valor</span><span class="sxs-lookup"><span data-stu-id="12459-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12459-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12459-122">Authorization</span></span>|<span data-ttu-id="12459-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12459-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12459-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12459-124">Accept</span></span>|<span data-ttu-id="12459-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12459-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12459-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12459-126">Request body</span></span>
<span data-ttu-id="12459-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12459-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12459-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12459-128">Response</span></span>
<span data-ttu-id="12459-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12459-129">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12459-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12459-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="12459-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12459-131">Request</span></span>
<span data-ttu-id="12459-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12459-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="12459-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="12459-133">Response</span></span>
<span data-ttu-id="12459-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12459-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1376

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsMobileMSI",
      "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "commandLine": "Command Line value",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "ignoreVersionDetection": true,
      "identityVersion": "Identity Version value",
      "useDeviceContext": true
    }
  ]
}
```




