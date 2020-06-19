---
title: Listar windowsFeatureUpdateProfileAssignments
description: Listar Propriedades e relações dos objetos windowsFeatureUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d3a5a3b3cc6126af4401aae7c569bf4538c7851
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791283"
---
# <a name="list-windowsfeatureupdateprofileassignments"></a><span data-ttu-id="fb051-103">Listar windowsFeatureUpdateProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="fb051-103">List windowsFeatureUpdateProfileAssignments</span></span>

<span data-ttu-id="fb051-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb051-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb051-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb051-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb051-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb051-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb051-107">Listar Propriedades e relações dos objetos [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fb051-107">List properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb051-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb051-108">Prerequisites</span></span>
<span data-ttu-id="fb051-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fb051-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fb051-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb051-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb051-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb051-111">Permission type</span></span>|<span data-ttu-id="fb051-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb051-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb051-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb051-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb051-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb051-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb051-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb051-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb051-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb051-116">Not supported.</span></span>|
|<span data-ttu-id="fb051-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb051-117">Application</span></span>|<span data-ttu-id="fb051-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb051-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb051-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb051-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fb051-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb051-120">Request headers</span></span>
|<span data-ttu-id="fb051-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb051-121">Header</span></span>|<span data-ttu-id="fb051-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb051-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb051-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb051-123">Authorization</span></span>|<span data-ttu-id="fb051-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb051-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb051-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb051-125">Accept</span></span>|<span data-ttu-id="fb051-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb051-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb051-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb051-127">Request body</span></span>
<span data-ttu-id="fb051-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb051-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb051-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb051-129">Response</span></span>
<span data-ttu-id="fb051-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb051-130">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb051-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb051-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb051-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb051-132">Request</span></span>
<span data-ttu-id="fb051-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb051-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="fb051-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb051-134">Response</span></span>
<span data-ttu-id="fb051-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fb051-135">Here is an example of the response.</span></span> <span data-ttu-id="fb051-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fb051-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fb051-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fb051-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
      "id": "567a744f-744f-567a-4f74-7a564f747a56",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



