---
title: Listar windowsPhone81StoreApps
description: Listar Propriedades e relações dos objetos windowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aaa9a519a572044c4546331c8962007f69f2dcce
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726250"
---
# <a name="list-windowsphone81storeapps"></a><span data-ttu-id="8979e-103">Listar windowsPhone81StoreApps</span><span class="sxs-lookup"><span data-stu-id="8979e-103">List windowsPhone81StoreApps</span></span>

<span data-ttu-id="8979e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8979e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8979e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8979e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8979e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8979e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8979e-107">Listar Propriedades e relações dos objetos [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8979e-107">List properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8979e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8979e-108">Prerequisites</span></span>
<span data-ttu-id="8979e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8979e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8979e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8979e-111">Permission type</span></span>|<span data-ttu-id="8979e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8979e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8979e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8979e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8979e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8979e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8979e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8979e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8979e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8979e-116">Not supported.</span></span>|
|<span data-ttu-id="8979e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8979e-117">Application</span></span>|<span data-ttu-id="8979e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8979e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8979e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8979e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8979e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8979e-120">Request headers</span></span>
|<span data-ttu-id="8979e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8979e-121">Header</span></span>|<span data-ttu-id="8979e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8979e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8979e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8979e-123">Authorization</span></span>|<span data-ttu-id="8979e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8979e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8979e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8979e-125">Accept</span></span>|<span data-ttu-id="8979e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8979e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8979e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8979e-127">Request body</span></span>
<span data-ttu-id="8979e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8979e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8979e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8979e-129">Response</span></span>
<span data-ttu-id="8979e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8979e-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8979e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8979e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8979e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8979e-132">Request</span></span>
<span data-ttu-id="8979e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8979e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8979e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8979e-134">Response</span></span>
<span data-ttu-id="8979e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8979e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

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
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





