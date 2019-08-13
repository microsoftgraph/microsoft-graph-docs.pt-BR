---
title: Listar roleScopeTagAutoAssignments
description: Listar Propriedades e relações dos objetos roleScopeTagAutoAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57c26411158bc9b7ae147f31fedaa3fadded175c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347623"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="37340-103">Listar roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="37340-103">List roleScopeTagAutoAssignments</span></span>

> <span data-ttu-id="37340-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37340-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37340-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37340-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37340-106">Listar Propriedades e relações dos objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="37340-106">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37340-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37340-107">Prerequisites</span></span>
<span data-ttu-id="37340-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37340-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37340-110">Permission type</span></span>|<span data-ttu-id="37340-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37340-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37340-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37340-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37340-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="37340-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="37340-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37340-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37340-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37340-115">Not supported.</span></span>|
|<span data-ttu-id="37340-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37340-116">Application</span></span>|<span data-ttu-id="37340-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="37340-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37340-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37340-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="37340-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37340-119">Request headers</span></span>
|<span data-ttu-id="37340-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37340-120">Header</span></span>|<span data-ttu-id="37340-121">Valor</span><span class="sxs-lookup"><span data-stu-id="37340-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37340-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37340-122">Authorization</span></span>|<span data-ttu-id="37340-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37340-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37340-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37340-124">Accept</span></span>|<span data-ttu-id="37340-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37340-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37340-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37340-126">Request body</span></span>
<span data-ttu-id="37340-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37340-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37340-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="37340-128">Response</span></span>
<span data-ttu-id="37340-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37340-129">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37340-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37340-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="37340-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37340-131">Request</span></span>
<span data-ttu-id="37340-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37340-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="37340-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="37340-133">Response</span></span>
<span data-ttu-id="37340-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37340-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






