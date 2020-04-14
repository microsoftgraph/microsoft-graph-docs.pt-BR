---
title: Atualizar roleScopeTagAutoAssignment
description: Atualiza as propriedades de um objeto roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4c879c070b524a00c07ee6cae40ab0206c6875a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445211"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="7dc55-103">Atualizar roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="7dc55-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="7dc55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dc55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dc55-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dc55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dc55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dc55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dc55-107">Atualiza as propriedades de um objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc55-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dc55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dc55-108">Prerequisites</span></span>
<span data-ttu-id="7dc55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dc55-111">Permission type</span></span>|<span data-ttu-id="7dc55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7dc55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dc55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dc55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dc55-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc55-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7dc55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dc55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dc55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dc55-116">Not supported.</span></span>|
|<span data-ttu-id="7dc55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dc55-117">Application</span></span>|<span data-ttu-id="7dc55-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc55-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dc55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7dc55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc55-120">Request headers</span></span>
|<span data-ttu-id="7dc55-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dc55-121">Header</span></span>|<span data-ttu-id="7dc55-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7dc55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dc55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dc55-123">Authorization</span></span>|<span data-ttu-id="7dc55-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dc55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dc55-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dc55-125">Accept</span></span>|<span data-ttu-id="7dc55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dc55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc55-127">Request body</span></span>
<span data-ttu-id="7dc55-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc55-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="7dc55-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7dc55-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="7dc55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dc55-130">Property</span></span>|<span data-ttu-id="7dc55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dc55-131">Type</span></span>|<span data-ttu-id="7dc55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dc55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dc55-133">id</span><span class="sxs-lookup"><span data-stu-id="7dc55-133">id</span></span>|<span data-ttu-id="7dc55-134">String</span><span class="sxs-lookup"><span data-stu-id="7dc55-134">String</span></span>|<span data-ttu-id="7dc55-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7dc55-135">Key of the entity.</span></span>|
|<span data-ttu-id="7dc55-136">destino</span><span class="sxs-lookup"><span data-stu-id="7dc55-136">target</span></span>|[<span data-ttu-id="7dc55-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7dc55-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7dc55-138">O destino da atribuição automática para a marca de escopo de função específica.</span><span class="sxs-lookup"><span data-stu-id="7dc55-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="7dc55-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc55-139">Response</span></span>
<span data-ttu-id="7dc55-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dc55-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dc55-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dc55-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dc55-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dc55-142">Request</span></span>
<span data-ttu-id="7dc55-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dc55-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7dc55-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dc55-144">Response</span></span>
<span data-ttu-id="7dc55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dc55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



