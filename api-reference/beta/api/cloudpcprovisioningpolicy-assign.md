---
title: 'cloudPcProvisioningPolicy: assign'
description: Atribua a política de provisionamento do computador na nuvem ao seu grupo.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 46d9877b8a17056aee84f1216c4f38227bdc097c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082192"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="fa413-103">cloudPcProvisioningPolicy: assign</span><span class="sxs-lookup"><span data-stu-id="fa413-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="fa413-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa413-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa413-105">Atribua [cloudPcProvisioningPolicy a](../resources/cloudpcprovisioningpolicy.md) grupos de usuários.</span><span class="sxs-lookup"><span data-stu-id="fa413-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="fa413-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa413-106">Permissions</span></span>

<span data-ttu-id="fa413-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa413-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa413-109">Permission type</span></span>|<span data-ttu-id="fa413-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa413-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa413-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa413-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa413-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa413-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fa413-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa413-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa413-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa413-114">Not supported.</span></span>|
|<span data-ttu-id="fa413-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa413-115">Application</span></span>|<span data-ttu-id="fa413-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa413-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa413-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa413-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="fa413-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa413-118">Request headers</span></span>

|<span data-ttu-id="fa413-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fa413-119">Name</span></span>|<span data-ttu-id="fa413-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa413-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fa413-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa413-121">Authorization</span></span>|<span data-ttu-id="fa413-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa413-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fa413-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa413-124">Content-Type</span></span>|<span data-ttu-id="fa413-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa413-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa413-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa413-127">Request body</span></span>

<span data-ttu-id="fa413-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcProvisioningPolicyAssignment.](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fa413-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

|<span data-ttu-id="fa413-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa413-129">Parameter</span></span>|<span data-ttu-id="fa413-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa413-130">Type</span></span>|<span data-ttu-id="fa413-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa413-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa413-132">assignments</span><span class="sxs-lookup"><span data-stu-id="fa413-132">assignments</span></span>|<span data-ttu-id="fa413-133">[coleção cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fa413-133">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) collection</span></span> | <span data-ttu-id="fa413-134">A coleção de recursos de política de provisionamento de computadores na nuvem a serem atribuídos ao grupo de destino correspondente.</span><span class="sxs-lookup"><span data-stu-id="fa413-134">The collection of cloud PC provisioning policy resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="fa413-135">Atualmente, Microsoft 365 grupos de segurança e grupos de segurança no Azure AD são suportados.</span><span class="sxs-lookup"><span data-stu-id="fa413-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="fa413-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa413-136">Response</span></span>

<span data-ttu-id="fa413-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fa413-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fa413-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa413-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa413-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa413-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fa413-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa413-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fa413-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa413-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa413-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa413-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa413-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa413-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
