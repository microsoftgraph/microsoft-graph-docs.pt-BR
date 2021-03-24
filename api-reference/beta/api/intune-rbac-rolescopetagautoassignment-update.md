---
title: Atualizar roleScopeTagAutoAssignment
description: Atualize as propriedades de um objeto roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 919c9dee6eca38ee343809e13805ca8d3e623cac
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134470"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="6fea3-103">Atualizar roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="6fea3-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="6fea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fea3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fea3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fea3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fea3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fea3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fea3-107">Atualize as propriedades de [um objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fea3-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fea3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6fea3-108">Prerequisites</span></span>
<span data-ttu-id="6fea3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fea3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fea3-111">Permission type</span></span>|<span data-ttu-id="6fea3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fea3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fea3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fea3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fea3-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fea3-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6fea3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fea3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fea3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fea3-116">Not supported.</span></span>|
|<span data-ttu-id="6fea3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fea3-117">Application</span></span>|<span data-ttu-id="6fea3-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fea3-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fea3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fea3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6fea3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fea3-120">Request headers</span></span>
|<span data-ttu-id="6fea3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fea3-121">Header</span></span>|<span data-ttu-id="6fea3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6fea3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fea3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fea3-123">Authorization</span></span>|<span data-ttu-id="6fea3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fea3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fea3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6fea3-125">Accept</span></span>|<span data-ttu-id="6fea3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fea3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fea3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fea3-127">Request body</span></span>
<span data-ttu-id="6fea3-128">No corpo da solicitação, fornece uma representação JSON para o [objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fea3-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="6fea3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a funçãoScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6fea3-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="6fea3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fea3-130">Property</span></span>|<span data-ttu-id="6fea3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fea3-131">Type</span></span>|<span data-ttu-id="6fea3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fea3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fea3-133">id</span><span class="sxs-lookup"><span data-stu-id="6fea3-133">id</span></span>|<span data-ttu-id="6fea3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fea3-134">String</span></span>|<span data-ttu-id="6fea3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6fea3-135">Key of the entity.</span></span>|
|<span data-ttu-id="6fea3-136">destino</span><span class="sxs-lookup"><span data-stu-id="6fea3-136">target</span></span>|[<span data-ttu-id="6fea3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6fea3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6fea3-138">O destino da atribuição automática para a marca de escopo de função específica.</span><span class="sxs-lookup"><span data-stu-id="6fea3-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="6fea3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fea3-139">Response</span></span>
<span data-ttu-id="6fea3-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fea3-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fea3-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fea3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fea3-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fea3-142">Request</span></span>
<span data-ttu-id="6fea3-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fea3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6fea3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fea3-144">Response</span></span>
<span data-ttu-id="6fea3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fea3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




