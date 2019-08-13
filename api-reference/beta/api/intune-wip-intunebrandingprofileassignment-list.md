---
title: Listar intuneBrandingProfileAssignments
description: Listar Propriedades e relações dos objetos intuneBrandingProfileAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3557e2ba243f96ee52208f8a6724c300d6df98b4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347168"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="b2280-103">Listar intuneBrandingProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="b2280-103">List intuneBrandingProfileAssignments</span></span>

> <span data-ttu-id="b2280-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2280-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2280-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2280-106">Listar Propriedades e relações dos objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b2280-106">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2280-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2280-107">Prerequisites</span></span>
<span data-ttu-id="b2280-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2280-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2280-110">Permission type</span></span>|<span data-ttu-id="b2280-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2280-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2280-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2280-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2280-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2280-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b2280-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2280-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2280-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2280-115">Not supported.</span></span>|
|<span data-ttu-id="b2280-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2280-116">Application</span></span>|<span data-ttu-id="b2280-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2280-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2280-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2280-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b2280-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2280-119">Request headers</span></span>
|<span data-ttu-id="b2280-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2280-120">Header</span></span>|<span data-ttu-id="b2280-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2280-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2280-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2280-122">Authorization</span></span>|<span data-ttu-id="b2280-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2280-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2280-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2280-124">Accept</span></span>|<span data-ttu-id="b2280-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2280-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2280-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2280-126">Request body</span></span>
<span data-ttu-id="b2280-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2280-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2280-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2280-128">Response</span></span>
<span data-ttu-id="b2280-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2280-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2280-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2280-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2280-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2280-131">Request</span></span>
<span data-ttu-id="b2280-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2280-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="b2280-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2280-133">Response</span></span>
<span data-ttu-id="b2280-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2280-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






