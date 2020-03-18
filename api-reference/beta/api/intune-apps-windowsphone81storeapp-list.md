---
title: Listar windowsPhone81StoreApps
description: Listar Propriedades e relações dos objetos windowsPhone81StoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b402ffddbdccfca65600388e8c0d751d603c8f20
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760750"
---
# <a name="list-windowsphone81storeapps"></a><span data-ttu-id="3aaa4-103">Listar windowsPhone81StoreApps</span><span class="sxs-lookup"><span data-stu-id="3aaa4-103">List windowsPhone81StoreApps</span></span>

> <span data-ttu-id="3aaa4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3aaa4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3aaa4-106">Listar Propriedades e relações dos objetos [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3aaa4-106">List properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3aaa4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3aaa4-107">Prerequisites</span></span>
<span data-ttu-id="3aaa4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aaa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aaa4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aaa4-110">Permission type</span></span>|<span data-ttu-id="3aaa4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3aaa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aaa4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aaa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3aaa4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aaa4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3aaa4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aaa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aaa4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-115">Not supported.</span></span>|
|<span data-ttu-id="3aaa4-116">Application</span><span class="sxs-lookup"><span data-stu-id="3aaa4-116">Application</span></span>|<span data-ttu-id="3aaa4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aaa4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aaa4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aaa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3aaa4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaa4-119">Request headers</span></span>
|<span data-ttu-id="3aaa4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3aaa4-120">Header</span></span>|<span data-ttu-id="3aaa4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3aaa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aaa4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aaa4-122">Authorization</span></span>|<span data-ttu-id="3aaa4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aaa4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3aaa4-124">Accept</span></span>|<span data-ttu-id="3aaa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3aaa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aaa4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaa4-126">Request body</span></span>
<span data-ttu-id="3aaa4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aaa4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaa4-128">Response</span></span>
<span data-ttu-id="3aaa4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aaa4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aaa4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3aaa4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aaa4-131">Request</span></span>
<span data-ttu-id="3aaa4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="3aaa4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aaa4-133">Response</span></span>
<span data-ttu-id="3aaa4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aaa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1084

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
      "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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




