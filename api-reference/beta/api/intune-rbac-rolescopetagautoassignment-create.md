---
title: Criar roleScopeTagAutoAssignment
description: Criar um novo objeto roleScopeTagAutoAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46c2f1442910a3ab6d3358829f77bae01eeaa391
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194899"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="187f8-103">Criar roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="187f8-103">Create roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="187f8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="187f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="187f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="187f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="187f8-106">Criar um novo objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="187f8-106">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="187f8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="187f8-107">Prerequisites</span></span>
<span data-ttu-id="187f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="187f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="187f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="187f8-110">Permission type</span></span>|<span data-ttu-id="187f8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="187f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="187f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="187f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="187f8-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187f8-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="187f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="187f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="187f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="187f8-115">Not supported.</span></span>|
|<span data-ttu-id="187f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="187f8-116">Application</span></span>|<span data-ttu-id="187f8-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187f8-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="187f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="187f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="187f8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="187f8-119">Request headers</span></span>
|<span data-ttu-id="187f8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="187f8-120">Header</span></span>|<span data-ttu-id="187f8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="187f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="187f8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="187f8-122">Authorization</span></span>|<span data-ttu-id="187f8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="187f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="187f8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="187f8-124">Accept</span></span>|<span data-ttu-id="187f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="187f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="187f8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="187f8-126">Request body</span></span>
<span data-ttu-id="187f8-127">No corpo da solicitação, forneça uma representação JSON do objeto roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="187f8-127">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="187f8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="187f8-128">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="187f8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="187f8-129">Property</span></span>|<span data-ttu-id="187f8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="187f8-130">Type</span></span>|<span data-ttu-id="187f8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="187f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="187f8-132">id</span><span class="sxs-lookup"><span data-stu-id="187f8-132">id</span></span>|<span data-ttu-id="187f8-133">String</span><span class="sxs-lookup"><span data-stu-id="187f8-133">String</span></span>|<span data-ttu-id="187f8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="187f8-134">Key of the entity.</span></span>|
|<span data-ttu-id="187f8-135">destino</span><span class="sxs-lookup"><span data-stu-id="187f8-135">target</span></span>|[<span data-ttu-id="187f8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="187f8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="187f8-137">O destino da atribuição automática para a marca de escopo de função específica.</span><span class="sxs-lookup"><span data-stu-id="187f8-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="187f8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="187f8-138">Response</span></span>
<span data-ttu-id="187f8-139">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="187f8-139">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="187f8-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="187f8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="187f8-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="187f8-141">Request</span></span>
<span data-ttu-id="187f8-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="187f8-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="187f8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="187f8-143">Response</span></span>
<span data-ttu-id="187f8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="187f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




