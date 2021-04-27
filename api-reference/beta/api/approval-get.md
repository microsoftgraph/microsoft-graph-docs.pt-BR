---
title: Obter aprovação
description: Recupere as propriedades de um objeto de aprovação.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 505133c6f26835440a0834b6553904562e449914
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048061"
---
# <a name="get-approval"></a><span data-ttu-id="9c897-103">Obter aprovação</span><span class="sxs-lookup"><span data-stu-id="9c897-103">Get approval</span></span>

<span data-ttu-id="9c897-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c897-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupera as propriedades de um [objeto de aprovação.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="9c897-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieves the properties of an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="9c897-106">Essa chamada pode ser feita por um aprovador, fornecendo o identificador da solicitação de atribuição [do pacote de acesso.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9c897-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c897-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c897-107">Permissions</span></span>

<span data-ttu-id="9c897-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c897-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c897-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c897-110">Permission type</span></span>                        | <span data-ttu-id="9c897-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c897-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9c897-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c897-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c897-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c897-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9c897-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c897-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c897-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c897-115">Not supported.</span></span> |
| <span data-ttu-id="9c897-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c897-116">Application</span></span>                            | <span data-ttu-id="9c897-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c897-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c897-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c897-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9c897-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c897-119">Request headers</span></span>

| <span data-ttu-id="9c897-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9c897-120">Name</span></span>      |<span data-ttu-id="9c897-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c897-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c897-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c897-122">Authorization</span></span> | <span data-ttu-id="9c897-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c897-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c897-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c897-125">Request body</span></span>

<span data-ttu-id="9c897-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c897-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c897-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c897-127">Response</span></span>

<span data-ttu-id="9c897-128">Se tiver êxito, este método retornará um código de resposta e o objeto de aprovação `200 OK` solicitado no corpo da resposta. [](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="9c897-128">If successful, this method returns a `200 OK` response code and the requested [approval](../resources/approval.md) object in the response body.</span></span> <span data-ttu-id="9c897-129">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c897-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9c897-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c897-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c897-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c897-131">Request</span></span>

<span data-ttu-id="9c897-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c897-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c897-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c897-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approval"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489
```
# <a name="c"></a>[<span data-ttu-id="9c897-134">C#</span><span class="sxs-lookup"><span data-stu-id="9c897-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c897-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c897-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c897-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c897-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c897-137">Java</span><span class="sxs-lookup"><span data-stu-id="9c897-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="9c897-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c897-138">Response</span></span>

<span data-ttu-id="9c897-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c897-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9c897-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c897-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approval"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "abd306ef-f7b2-4a10-9fd1-493454322489",
    "steps": [
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
  "description": "Get approval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


