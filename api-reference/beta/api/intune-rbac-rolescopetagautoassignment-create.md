---
title: Criar roleScopeTagAutoAssignment
description: Crie um novo objeto roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9aec4bccfd129da624a3f12691704d273f8f1d4b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159280"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="bb56d-103">Criar roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="bb56d-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="bb56d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb56d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb56d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb56d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb56d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb56d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb56d-107">Crie um novo [objeto roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bb56d-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb56d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb56d-108">Prerequisites</span></span>
<span data-ttu-id="bb56d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb56d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb56d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb56d-111">Permission type</span></span>|<span data-ttu-id="bb56d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb56d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb56d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb56d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb56d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb56d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="bb56d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb56d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb56d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb56d-116">Not supported.</span></span>|
|<span data-ttu-id="bb56d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb56d-117">Application</span></span>|<span data-ttu-id="bb56d-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb56d-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb56d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb56d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bb56d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb56d-120">Request headers</span></span>
|<span data-ttu-id="bb56d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb56d-121">Header</span></span>|<span data-ttu-id="bb56d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb56d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb56d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb56d-123">Authorization</span></span>|<span data-ttu-id="bb56d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb56d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb56d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb56d-125">Accept</span></span>|<span data-ttu-id="bb56d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb56d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb56d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb56d-127">Request body</span></span>
<span data-ttu-id="bb56d-128">No corpo da solicitação, fornece uma representação JSON do objeto roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="bb56d-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="bb56d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="bb56d-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="bb56d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb56d-130">Property</span></span>|<span data-ttu-id="bb56d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb56d-131">Type</span></span>|<span data-ttu-id="bb56d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb56d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb56d-133">id</span><span class="sxs-lookup"><span data-stu-id="bb56d-133">id</span></span>|<span data-ttu-id="bb56d-134">String</span><span class="sxs-lookup"><span data-stu-id="bb56d-134">String</span></span>|<span data-ttu-id="bb56d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb56d-135">Key of the entity.</span></span>|
|<span data-ttu-id="bb56d-136">destino</span><span class="sxs-lookup"><span data-stu-id="bb56d-136">target</span></span>|[<span data-ttu-id="bb56d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb56d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bb56d-138">O destino de atribuição automática para a Marca de Escopo de Função específica.</span><span class="sxs-lookup"><span data-stu-id="bb56d-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="bb56d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb56d-139">Response</span></span>
<span data-ttu-id="bb56d-140">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb56d-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb56d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb56d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb56d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb56d-142">Request</span></span>
<span data-ttu-id="bb56d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb56d-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb56d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb56d-144">Response</span></span>
<span data-ttu-id="bb56d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb56d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




