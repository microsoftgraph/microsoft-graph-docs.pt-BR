---
title: Listar intuneBrandingProfileAssignments
description: Listar Propriedades e relações dos objetos intuneBrandingProfileAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d75a9317b721122486313edeb33f6b85c3cc60a8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799678"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="4f996-103">Listar intuneBrandingProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="4f996-103">List intuneBrandingProfileAssignments</span></span>

> <span data-ttu-id="4f996-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f996-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f996-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f996-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f996-106">Listar Propriedades e relações dos objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4f996-106">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f996-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f996-107">Prerequisites</span></span>
<span data-ttu-id="4f996-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f996-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f996-110">Permission type</span></span>|<span data-ttu-id="4f996-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f996-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f996-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f996-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f996-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f996-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4f996-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f996-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f996-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f996-115">Not supported.</span></span>|
|<span data-ttu-id="4f996-116">Application</span><span class="sxs-lookup"><span data-stu-id="4f996-116">Application</span></span>|<span data-ttu-id="4f996-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f996-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f996-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f996-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4f996-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f996-119">Request headers</span></span>
|<span data-ttu-id="4f996-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f996-120">Header</span></span>|<span data-ttu-id="4f996-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f996-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f996-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f996-122">Authorization</span></span>|<span data-ttu-id="4f996-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f996-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f996-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f996-124">Accept</span></span>|<span data-ttu-id="4f996-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f996-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f996-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f996-126">Request body</span></span>
<span data-ttu-id="4f996-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f996-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f996-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f996-128">Response</span></span>
<span data-ttu-id="4f996-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f996-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f996-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f996-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f996-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f996-131">Request</span></span>
<span data-ttu-id="4f996-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f996-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="4f996-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f996-133">Response</span></span>
<span data-ttu-id="4f996-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f996-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




