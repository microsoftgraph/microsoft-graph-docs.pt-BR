---
title: Aprovação de listaSteps
description: Listar etapas de aprovação associadas a um objeto de aprovação.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 797d2715dd2c273c5673e608a4794fc0c56a6f45
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961356"
---
# <a name="list-approvalsteps"></a><span data-ttu-id="16200-103">Aprovação de listaSteps</span><span class="sxs-lookup"><span data-stu-id="16200-103">List approvalSteps</span></span>

<span data-ttu-id="16200-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16200-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16200-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)lista os objetos [approvalStep](../resources/approvalstep.md) associados a um [objeto de aprovação.](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="16200-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), lists the [approvalStep](../resources/approvalstep.md) objects associated with an [approval](../resources/approval.md) object.</span></span>  <span data-ttu-id="16200-106">Essa chamada pode ser feita por um aprovador, fornecendo o identificador da solicitação de atribuição [do pacote de acesso.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="16200-106">This call can be made by an approver, providing the identifier of the [access package assignment request](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16200-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16200-107">Permissions</span></span>

<span data-ttu-id="16200-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16200-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16200-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16200-110">Permission type</span></span>                        | <span data-ttu-id="16200-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16200-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="16200-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16200-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="16200-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16200-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="16200-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16200-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16200-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16200-115">Not supported.</span></span> |
| <span data-ttu-id="16200-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16200-116">Application</span></span>                            | <span data-ttu-id="16200-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16200-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16200-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16200-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps
```

## <a name="request-headers"></a><span data-ttu-id="16200-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16200-119">Request headers</span></span>

| <span data-ttu-id="16200-120">Nome</span><span class="sxs-lookup"><span data-stu-id="16200-120">Name</span></span>      |<span data-ttu-id="16200-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="16200-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16200-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16200-122">Authorization</span></span> | <span data-ttu-id="16200-123">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="16200-123">Bearer \{token\}.</span></span> <span data-ttu-id="16200-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16200-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16200-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16200-125">Request body</span></span>

<span data-ttu-id="16200-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16200-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16200-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="16200-127">Response</span></span>

<span data-ttu-id="16200-128">Se tiver êxito, este método retornará um código de resposta e uma coleção dos objetos `200 OK` [approvalStep](../resources/approvalstep.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16200-128">If successful, this method returns a `200 OK` response code and a collection of the [approvalStep](../resources/approvalstep.md) objects in the response body.</span></span> <span data-ttu-id="16200-129">No entanto, se o chamador não tiver as permissões certas, o método retornará um `403 Forbidden` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="16200-129">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="16200-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16200-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16200-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16200-131">Request</span></span>

<span data-ttu-id="16200-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16200-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="16200-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="16200-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approvalstep_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps
```
# <a name="c"></a>[<span data-ttu-id="16200-134">C#</span><span class="sxs-lookup"><span data-stu-id="16200-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approvalstep-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16200-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16200-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approvalstep-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16200-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16200-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approvalstep-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16200-137">Java</span><span class="sxs-lookup"><span data-stu-id="16200-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approvalstep-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="16200-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="16200-138">Response</span></span>

<span data-ttu-id="16200-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16200-139">The following is an example of the response.</span></span>

> <span data-ttu-id="16200-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16200-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


