---
title: Listar windowsPhone81AppXs
description: Listar Propriedades e relações dos objetos windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 935e26445f2e6de51228e658f80aae51aefb2427
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149284"
---
# <a name="list-windowsphone81appxs"></a><span data-ttu-id="f3685-103">Listar windowsPhone81AppXs</span><span class="sxs-lookup"><span data-stu-id="f3685-103">List windowsPhone81AppXs</span></span>

> <span data-ttu-id="f3685-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3685-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3685-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3685-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3685-106">Listar Propriedades e relações dos objetos [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="f3685-106">List properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3685-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3685-107">Prerequisites</span></span>
<span data-ttu-id="f3685-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3685-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3685-110">Permission type</span></span>|<span data-ttu-id="f3685-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3685-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3685-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3685-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3685-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3685-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3685-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3685-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3685-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3685-115">Not supported.</span></span>|
|<span data-ttu-id="f3685-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3685-116">Application</span></span>|<span data-ttu-id="f3685-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3685-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3685-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3685-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f3685-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3685-119">Request headers</span></span>
|<span data-ttu-id="f3685-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3685-120">Header</span></span>|<span data-ttu-id="f3685-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f3685-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3685-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3685-122">Authorization</span></span>|<span data-ttu-id="f3685-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3685-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3685-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3685-124">Accept</span></span>|<span data-ttu-id="f3685-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3685-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3685-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3685-126">Request body</span></span>
<span data-ttu-id="f3685-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3685-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3685-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3685-128">Response</span></span>
<span data-ttu-id="f3685-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3685-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3685-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3685-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3685-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3685-131">Request</span></span>
<span data-ttu-id="f3685-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3685-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f3685-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3685-133">Response</span></span>
<span data-ttu-id="f3685-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3685-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1821

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81AppX",
      "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
      "applicableArchitectures": "x86",
      "identityName": "Identity Name value",
      "identityPublisherHash": "Identity Publisher Hash value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
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
      "phoneProductIdentifier": "Phone Product Identifier value",
      "phonePublisherId": "Phone Publisher Id value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




