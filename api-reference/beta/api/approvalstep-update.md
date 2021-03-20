---
title: Atualizar approvalStep
description: Aplicar aprovar ou negar decisão em um objeto approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b8ef436a9319e7a670e0aa5bdc728b39b53c2709
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942517"
---
# <a name="update-approvalstep"></a><span data-ttu-id="f86cb-103">Atualizar approvalStep</span><span class="sxs-lookup"><span data-stu-id="f86cb-103">Update approvalStep</span></span>

<span data-ttu-id="f86cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f86cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f86cb-105">Aplicar aprovar ou negar decisão em um [objeto approvalStep.](../resources/approvalStep.md)</span><span class="sxs-lookup"><span data-stu-id="f86cb-105">Apply approve or deny decision on an [approvalStep](../resources/approvalStep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f86cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f86cb-106">Permissions</span></span>

<span data-ttu-id="f86cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f86cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f86cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f86cb-109">Permission type</span></span>                        | <span data-ttu-id="f86cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f86cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f86cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f86cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f86cb-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f86cb-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f86cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f86cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f86cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f86cb-114">Not supported.</span></span> |
| <span data-ttu-id="f86cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f86cb-115">Application</span></span>                            | <span data-ttu-id="f86cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f86cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f86cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f86cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f86cb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f86cb-118">Request headers</span></span>

| <span data-ttu-id="f86cb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f86cb-119">Name</span></span>      |<span data-ttu-id="f86cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f86cb-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f86cb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f86cb-121">Authorization</span></span> | <span data-ttu-id="f86cb-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="f86cb-122">Bearer \{token\}.</span></span> <span data-ttu-id="f86cb-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f86cb-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f86cb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f86cb-124">Request body</span></span>

<span data-ttu-id="f86cb-125">A tabela a seguir mostra as propriedades necessárias para este método.</span><span class="sxs-lookup"><span data-stu-id="f86cb-125">The following table shows the properties that are required for this method.</span></span>

| <span data-ttu-id="f86cb-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f86cb-126">Property</span></span>       | <span data-ttu-id="f86cb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f86cb-127">Type</span></span>    |<span data-ttu-id="f86cb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f86cb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f86cb-129">reviewResult</span><span class="sxs-lookup"><span data-stu-id="f86cb-129">reviewResult</span></span> | <span data-ttu-id="f86cb-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f86cb-130">String</span></span> | <span data-ttu-id="f86cb-131">Decisão do aprovador.</span><span class="sxs-lookup"><span data-stu-id="f86cb-131">Decision of the approver.</span></span> <span data-ttu-id="f86cb-132">Os valores possíveis são: `Approve` e `Deny`.</span><span class="sxs-lookup"><span data-stu-id="f86cb-132">Possible values are: `Approve`, `Deny`.</span></span>|
| <span data-ttu-id="f86cb-133">justification</span><span class="sxs-lookup"><span data-stu-id="f86cb-133">justification</span></span> | <span data-ttu-id="f86cb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f86cb-134">String</span></span> | <span data-ttu-id="f86cb-135">Justificativa relacionada à decisão do aprovador.</span><span class="sxs-lookup"><span data-stu-id="f86cb-135">Justification related to the approver's decision.</span></span> |


## <a name="response"></a><span data-ttu-id="f86cb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f86cb-136">Response</span></span>

<span data-ttu-id="f86cb-137">Se tiver êxito, este método retornará `204 No Content` um código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f86cb-137">If successful, this method returns a `204 No Content` response code in the response body.</span></span> <span data-ttu-id="f86cb-138">No entanto, se o chamador não tiver as permissões certas, o método retornará um código de resposta ou se a id de aprovação não for encontrada, o `403 Forbidden` método retornará `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="f86cb-138">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code, or if the approval id is not found, the method returns `404 Not found`.</span></span> <span data-ttu-id="f86cb-139">Se a solicitação já tiver sido aprovada por outro aprovador no mesmo estágio de aprovação, o método `409 Conflict` retornará no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f86cb-139">If the request has already been approved by another approver in the same approval stage, the method returns `409 Conflict` in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f86cb-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f86cb-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f86cb-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f86cb-141">Request</span></span>

<span data-ttu-id="f86cb-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f86cb-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f86cb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f86cb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstep"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="objective-c"></a>[<span data-ttu-id="f86cb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f86cb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstep-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="f86cb-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f86cb-145">Response</span></span>

<span data-ttu-id="f86cb-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f86cb-146">The following is an example of the response.</span></span>

> <span data-ttu-id="f86cb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f86cb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-Type: application/json
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
