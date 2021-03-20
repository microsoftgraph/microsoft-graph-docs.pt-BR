---
title: Obter approvalStep
description: Recupere as propriedades de um objeto approvalStep.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7cc5d37c5dea66bc90661bf23b75ea43d82bc82e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942532"
---
# <a name="get-approvalstep"></a><span data-ttu-id="d399f-103">Obter approvalStep</span><span class="sxs-lookup"><span data-stu-id="d399f-103">Get approvalStep</span></span>

<span data-ttu-id="d399f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d399f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d399f-105">Recupere as propriedades de um [objeto approvalStep.](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="d399f-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d399f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d399f-106">Permissions</span></span>

<span data-ttu-id="d399f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d399f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d399f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d399f-109">Permission type</span></span>                        | <span data-ttu-id="d399f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d399f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d399f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d399f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d399f-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d399f-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d399f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d399f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d399f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d399f-114">Not supported.</span></span> |
| <span data-ttu-id="d399f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d399f-115">Application</span></span>                            | <span data-ttu-id="d399f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d399f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d399f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d399f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d399f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d399f-118">Request headers</span></span>

| <span data-ttu-id="d399f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d399f-119">Name</span></span>      |<span data-ttu-id="d399f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d399f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d399f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d399f-121">Authorization</span></span> | <span data-ttu-id="d399f-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="d399f-122">Bearer \{token\}.</span></span> <span data-ttu-id="d399f-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d399f-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d399f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d399f-124">Request body</span></span>

<span data-ttu-id="d399f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d399f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d399f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d399f-126">Response</span></span>

<span data-ttu-id="d399f-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [approvalStep](../resources/approvalstep.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d399f-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="d399f-128">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="d399f-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d399f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d399f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d399f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d399f-130">Request</span></span>

<span data-ttu-id="d399f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d399f-131">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="d399f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d399f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
# <a name="c"></a>[<span data-ttu-id="d399f-133">C#</span><span class="sxs-lookup"><span data-stu-id="d399f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d399f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d399f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d399f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d399f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d399f-136">Java</span><span class="sxs-lookup"><span data-stu-id="d399f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d399f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d399f-137">Response</span></span>

<span data-ttu-id="d399f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d399f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d399f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d399f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


