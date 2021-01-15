---
title: 'cloudPcProvisioningPolicy: assign'
description: Atribua a política de provisionamento do computador na nuvem ao seu grupo.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4b6acff15539c2a1b42f66547289621a7e87d7b5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872740"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="4759b-103">cloudPcProvisioningPolicy: assign</span><span class="sxs-lookup"><span data-stu-id="4759b-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="4759b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4759b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4759b-105">Atribua [cloudPcProvisioningPolicy a](../resources/cloudpcprovisioningpolicy.md) grupos de usuários.</span><span class="sxs-lookup"><span data-stu-id="4759b-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="4759b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4759b-106">Permissions</span></span>

<span data-ttu-id="4759b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4759b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4759b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4759b-109">Permission type</span></span>|<span data-ttu-id="4759b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4759b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4759b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4759b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4759b-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4759b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="4759b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4759b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4759b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4759b-114">Not supported.</span></span>|
|<span data-ttu-id="4759b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4759b-115">Application</span></span>|<span data-ttu-id="4759b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4759b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4759b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4759b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4759b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4759b-118">Request headers</span></span>

|<span data-ttu-id="4759b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4759b-119">Name</span></span>|<span data-ttu-id="4759b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4759b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4759b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4759b-121">Authorization</span></span>|<span data-ttu-id="4759b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4759b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4759b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4759b-124">Content-Type</span></span>|<span data-ttu-id="4759b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4759b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4759b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4759b-127">Request body</span></span>

<span data-ttu-id="4759b-128">No corpo da solicitação, fornece uma representação JSON do objeto [cloudPcProvisioningPolicyAssignment.](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4759b-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

<span data-ttu-id="4759b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4759b-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).</span></span>

|<span data-ttu-id="4759b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4759b-130">Property</span></span>|<span data-ttu-id="4759b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4759b-131">Type</span></span>|<span data-ttu-id="4759b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4759b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4759b-133">id</span><span class="sxs-lookup"><span data-stu-id="4759b-133">id</span></span>|<span data-ttu-id="4759b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4759b-134">String</span></span>|<span data-ttu-id="4759b-135">A ID da atribuição de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4759b-135">The ID of the provisioning policy assignment.</span></span> <span data-ttu-id="4759b-136">Se o destino for um grupo de usuários, a ID será mostrada como {policyId}_{groupId}.</span><span class="sxs-lookup"><span data-stu-id="4759b-136">If target is a user group, then the ID is shown as {policyId}_{groupId}.</span></span> |
|<span data-ttu-id="4759b-137">destino</span><span class="sxs-lookup"><span data-stu-id="4759b-137">target</span></span>|[<span data-ttu-id="4759b-138">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4759b-138">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="4759b-139">O destino da atribuição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4759b-139">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="4759b-140">Atualmente, o único destino com suporte é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="4759b-140">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="4759b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4759b-141">Response</span></span>

<span data-ttu-id="4759b-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4759b-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4759b-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4759b-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4759b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4759b-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4759b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4759b-145">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="4759b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4759b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4759b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4759b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4759b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4759b-148">Response</span></span>

<span data-ttu-id="4759b-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4759b-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
