---
title: Criar roleScopeTagAutoAssignment
description: Crie um novo objeto roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 498ab9824fac01efab4dae5f3d1418d3d175bfef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134533"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="4e5a8-103">Criar roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="4e5a8-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="4e5a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e5a8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e5a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e5a8-107">Crie um novo [objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4e5a8-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e5a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e5a8-108">Prerequisites</span></span>
<span data-ttu-id="4e5a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e5a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e5a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e5a8-111">Permission type</span></span>|<span data-ttu-id="4e5a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e5a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e5a8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e5a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e5a8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5a8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4e5a8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e5a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e5a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-116">Not supported.</span></span>|
|<span data-ttu-id="4e5a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e5a8-117">Application</span></span>|<span data-ttu-id="4e5a8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5a8-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e5a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e5a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4e5a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5a8-120">Request headers</span></span>
|<span data-ttu-id="4e5a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e5a8-121">Header</span></span>|<span data-ttu-id="4e5a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4e5a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e5a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e5a8-123">Authorization</span></span>|<span data-ttu-id="4e5a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e5a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e5a8-125">Accept</span></span>|<span data-ttu-id="4e5a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e5a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e5a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5a8-127">Request body</span></span>
<span data-ttu-id="4e5a8-128">No corpo da solicitação, fornece uma representação JSON para o objeto roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="4e5a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar a funçãoScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="4e5a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e5a8-130">Property</span></span>|<span data-ttu-id="4e5a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e5a8-131">Type</span></span>|<span data-ttu-id="4e5a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e5a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e5a8-133">id</span><span class="sxs-lookup"><span data-stu-id="4e5a8-133">id</span></span>|<span data-ttu-id="4e5a8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e5a8-134">String</span></span>|<span data-ttu-id="4e5a8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-135">Key of the entity.</span></span>|
|<span data-ttu-id="4e5a8-136">destino</span><span class="sxs-lookup"><span data-stu-id="4e5a8-136">target</span></span>|[<span data-ttu-id="4e5a8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4e5a8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4e5a8-138">O destino da atribuição automática para a marca de escopo de função específica.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="4e5a8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e5a8-139">Response</span></span>
<span data-ttu-id="4e5a8-140">Se tiver êxito, este método retornará um código de `201 Created` resposta e um objeto [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e5a8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e5a8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e5a8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e5a8-142">Request</span></span>
<span data-ttu-id="4e5a8-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
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

### <a name="response"></a><span data-ttu-id="4e5a8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e5a8-144">Response</span></span>
<span data-ttu-id="4e5a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e5a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




