---
title: Listar roleScopeTagAutoAssignments
description: Listar Propriedades e relações dos objetos roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c04669c1db70604fcd1edd3f1181b76248fd635
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791374"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="a4067-103">Listar roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="a4067-103">List roleScopeTagAutoAssignments</span></span>

<span data-ttu-id="a4067-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4067-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4067-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4067-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4067-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4067-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4067-107">Listar Propriedades e relações dos objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a4067-107">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4067-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4067-108">Prerequisites</span></span>
<span data-ttu-id="a4067-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a4067-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a4067-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4067-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4067-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4067-111">Permission type</span></span>|<span data-ttu-id="a4067-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4067-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4067-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4067-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4067-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4067-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a4067-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4067-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4067-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4067-116">Not supported.</span></span>|
|<span data-ttu-id="a4067-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4067-117">Application</span></span>|<span data-ttu-id="a4067-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4067-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4067-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4067-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a4067-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4067-120">Request headers</span></span>
|<span data-ttu-id="a4067-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4067-121">Header</span></span>|<span data-ttu-id="a4067-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a4067-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4067-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4067-123">Authorization</span></span>|<span data-ttu-id="a4067-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4067-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4067-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4067-125">Accept</span></span>|<span data-ttu-id="a4067-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4067-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4067-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4067-127">Request body</span></span>
<span data-ttu-id="a4067-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4067-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4067-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4067-129">Response</span></span>
<span data-ttu-id="a4067-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4067-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4067-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4067-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4067-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4067-132">Request</span></span>
<span data-ttu-id="a4067-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4067-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="a4067-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4067-134">Response</span></span>
<span data-ttu-id="a4067-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a4067-135">Here is an example of the response.</span></span> <span data-ttu-id="a4067-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a4067-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a4067-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a4067-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



