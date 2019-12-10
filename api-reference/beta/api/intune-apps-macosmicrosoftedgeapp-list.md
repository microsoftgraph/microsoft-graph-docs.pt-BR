---
title: Listar macOSMicrosoftEdgeApps
description: Listar Propriedades e relações dos objetos macOSMicrosoftEdgeApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f62cf6c6ea80972468e8a7ef2fbc2b7fdf4dc140
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39919553"
---
# <a name="list-macosmicrosoftedgeapps"></a><span data-ttu-id="2f3f2-103">Listar macOSMicrosoftEdgeApps</span><span class="sxs-lookup"><span data-stu-id="2f3f2-103">List macOSMicrosoftEdgeApps</span></span>

> <span data-ttu-id="2f3f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f3f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f3f2-106">Listar Propriedades e relações dos objetos [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2f3f2-106">List properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f3f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f3f2-107">Prerequisites</span></span>
<span data-ttu-id="2f3f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f3f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f3f2-110">Permission type</span></span>|<span data-ttu-id="2f3f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f3f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f3f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f3f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f3f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f3f2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f3f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f3f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f3f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-115">Not supported.</span></span>|
|<span data-ttu-id="2f3f2-116">Application</span><span class="sxs-lookup"><span data-stu-id="2f3f2-116">Application</span></span>|<span data-ttu-id="2f3f2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f3f2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f3f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f3f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f3f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3f2-119">Request headers</span></span>
|<span data-ttu-id="2f3f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f3f2-120">Header</span></span>|<span data-ttu-id="2f3f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f3f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f3f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f3f2-122">Authorization</span></span>|<span data-ttu-id="2f3f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f3f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f3f2-124">Accept</span></span>|<span data-ttu-id="2f3f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f3f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f3f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3f2-126">Request body</span></span>
<span data-ttu-id="2f3f2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f3f2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f3f2-128">Response</span></span>
<span data-ttu-id="2f3f2-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-129">If successful, this method returns a `200 OK` response code and a collection of [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f3f2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f3f2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f3f2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f3f2-131">Request</span></span>
<span data-ttu-id="2f3f2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2f3f2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f3f2-133">Response</span></span>
<span data-ttu-id="2f3f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f3f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
      "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
      "channel": "beta"
    }
  ]
}
```





