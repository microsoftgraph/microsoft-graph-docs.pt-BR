---
title: Listar windowsStoreApps
description: Listar Propriedades e relações dos objetos windowsStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd58dafffc0713d181197ae034cc1ed5cf86764f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805219"
---
# <a name="list-windowsstoreapps"></a><span data-ttu-id="2a16d-103">Listar windowsStoreApps</span><span class="sxs-lookup"><span data-stu-id="2a16d-103">List windowsStoreApps</span></span>

> <span data-ttu-id="2a16d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a16d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a16d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a16d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a16d-106">Listar Propriedades e relações dos objetos [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2a16d-106">List properties and relationships of the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a16d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a16d-107">Prerequisites</span></span>
<span data-ttu-id="2a16d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a16d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a16d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a16d-110">Permission type</span></span>|<span data-ttu-id="2a16d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a16d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a16d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a16d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a16d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a16d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2a16d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a16d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a16d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a16d-115">Not supported.</span></span>|
|<span data-ttu-id="2a16d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a16d-116">Application</span></span>|<span data-ttu-id="2a16d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a16d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a16d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a16d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2a16d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a16d-119">Request headers</span></span>
|<span data-ttu-id="2a16d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a16d-120">Header</span></span>|<span data-ttu-id="2a16d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a16d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a16d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a16d-122">Authorization</span></span>|<span data-ttu-id="2a16d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a16d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a16d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a16d-124">Accept</span></span>|<span data-ttu-id="2a16d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a16d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a16d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a16d-126">Request body</span></span>
<span data-ttu-id="2a16d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a16d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a16d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a16d-128">Response</span></span>
<span data-ttu-id="2a16d-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a16d-129">If successful, this method returns a `200 OK` response code and a collection of [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a16d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a16d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a16d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a16d-131">Request</span></span>
<span data-ttu-id="2a16d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a16d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2a16d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a16d-133">Response</span></span>
<span data-ttu-id="2a16d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a16d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1077

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsStoreApp",
      "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





