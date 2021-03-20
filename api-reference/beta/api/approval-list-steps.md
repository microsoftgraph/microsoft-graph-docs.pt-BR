---
title: Aprovação de listaSteps
description: Listar etapas de aprovação associadas a um objeto de aprovação.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 81df11f30ece700fc64361d7d6e9c154ed35eb49
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942566"
---
# <a name="list-approvalsteps"></a><span data-ttu-id="a70f9-103">Aprovação de listaSteps</span><span class="sxs-lookup"><span data-stu-id="a70f9-103">List approvalSteps</span></span>

<span data-ttu-id="a70f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a70f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a70f9-105">Listar [os objetos approvalStep](../resources/approvalstep.md) associados a um [objeto de](../resources/approval.md) aprovação.</span><span class="sxs-lookup"><span data-stu-id="a70f9-105">List the [approvalStep](../resources/approvalstep.md) objects associated with an [approval](../resources/approval.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a70f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a70f9-106">Permissions</span></span>

<span data-ttu-id="a70f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a70f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a70f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a70f9-109">Permission type</span></span>                        | <span data-ttu-id="a70f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a70f9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a70f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a70f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a70f9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70f9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a70f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a70f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a70f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a70f9-114">Not supported.</span></span> |
| <span data-ttu-id="a70f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a70f9-115">Application</span></span>                            | <span data-ttu-id="a70f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a70f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a70f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a70f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps
```

## <a name="request-headers"></a><span data-ttu-id="a70f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a70f9-118">Request headers</span></span>

| <span data-ttu-id="a70f9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a70f9-119">Name</span></span>      |<span data-ttu-id="a70f9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a70f9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a70f9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a70f9-121">Authorization</span></span> | <span data-ttu-id="a70f9-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="a70f9-122">Bearer \{token\}.</span></span> <span data-ttu-id="a70f9-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a70f9-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a70f9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a70f9-124">Request body</span></span>

<span data-ttu-id="a70f9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a70f9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a70f9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a70f9-126">Response</span></span>

<span data-ttu-id="a70f9-127">Se tiver êxito, este método retornará um código de resposta e uma coleção dos objetos `200 OK` [approvalStep](../resources/approvalstep.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a70f9-127">If successful, this method returns a `200 OK` response code and a collection of the [approvalStep](../resources/approvalstep.md) objects in the response body.</span></span> <span data-ttu-id="a70f9-128">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="a70f9-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a70f9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a70f9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a70f9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a70f9-130">Request</span></span>

<span data-ttu-id="a70f9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a70f9-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a70f9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a70f9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps
```
# <a name="c"></a>[<span data-ttu-id="a70f9-133">C#</span><span class="sxs-lookup"><span data-stu-id="a70f9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a70f9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a70f9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a70f9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a70f9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a70f9-136">Java</span><span class="sxs-lookup"><span data-stu-id="a70f9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="a70f9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a70f9-137">Response</span></span>

<span data-ttu-id="a70f9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a70f9-138">The following is an example of the response.</span></span>

> <span data-ttu-id="a70f9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a70f9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
            "displayName": null,
            "reviewedDateTime": null,
            "reviewResult": "NotReviewed",
            "status": "InProgress",
            "assignedToMe": true,
            "justification": "",
            "reviewedBy": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List approvalstep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


