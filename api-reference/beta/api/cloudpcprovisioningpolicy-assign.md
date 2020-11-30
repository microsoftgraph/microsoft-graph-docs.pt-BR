---
title: 'cloudPcProvisioningPolicy: assign'
description: Atribua a política de provisionamento do computador de nuvem ao grupo.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3e83fa363eeec142c194865da0bb0bef191aae50
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378212"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="30b7a-103">cloudPcProvisioningPolicy: assign</span><span class="sxs-lookup"><span data-stu-id="30b7a-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="30b7a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30b7a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30b7a-105">Atribuir [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) a grupos de usuários.</span><span class="sxs-lookup"><span data-stu-id="30b7a-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="30b7a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="30b7a-106">Permissions</span></span>

<span data-ttu-id="30b7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30b7a-109">Permission type</span></span>|<span data-ttu-id="30b7a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30b7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30b7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30b7a-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b7a-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="30b7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30b7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30b7a-114">Not supported.</span></span>|
|<span data-ttu-id="30b7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30b7a-115">Application</span></span>|<span data-ttu-id="30b7a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30b7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30b7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="30b7a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30b7a-118">Request headers</span></span>

|<span data-ttu-id="30b7a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="30b7a-119">Name</span></span>|<span data-ttu-id="30b7a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30b7a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30b7a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="30b7a-121">Authorization</span></span>|<span data-ttu-id="30b7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30b7a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="30b7a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30b7a-124">Content-Type</span></span>|<span data-ttu-id="30b7a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30b7a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b7a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30b7a-127">Request body</span></span>

<span data-ttu-id="30b7a-128">No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="30b7a-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="30b7a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="30b7a-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="30b7a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30b7a-130">Property</span></span>|<span data-ttu-id="30b7a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30b7a-131">Type</span></span>|<span data-ttu-id="30b7a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30b7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b7a-133">id</span><span class="sxs-lookup"><span data-stu-id="30b7a-133">id</span></span>|<span data-ttu-id="30b7a-134">String</span><span class="sxs-lookup"><span data-stu-id="30b7a-134">String</span></span>|<span data-ttu-id="30b7a-135">A ID da atribuição de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="30b7a-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="30b7a-136">Se target for um grupo de usuários, a ID será mostrada como {PolicyId} _ {GroupId}.</span><span class="sxs-lookup"><span data-stu-id="30b7a-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="30b7a-137">destino</span><span class="sxs-lookup"><span data-stu-id="30b7a-137">target</span></span>|[<span data-ttu-id="30b7a-138">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="30b7a-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="30b7a-139">O destino da atribuição para a política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="30b7a-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="30b7a-140">Atualmente, o único destino suportado é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="30b7a-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="30b7a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="30b7a-141">Response</span></span>

<span data-ttu-id="30b7a-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="30b7a-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="30b7a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30b7a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30b7a-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30b7a-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "assign_cloudpcprovisioningpolicy",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="30b7a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="30b7a-145">Response</span></span>

<span data-ttu-id="30b7a-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="30b7a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
