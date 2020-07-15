---
title: Atribuir tokenIssuancePolicy
description: Atribuir um tokenIssuancePolicy a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 649cb40d06d5a89cba9a07162410a71ebc54ca2e
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142217"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="9e972-103">Atribuir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="9e972-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="9e972-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e972-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e972-105">Atribuir um [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="9e972-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e972-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e972-106">Permissions</span></span>

<span data-ttu-id="9e972-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9e972-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9e972-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e972-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e972-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e972-109">Permission type</span></span>                        | <span data-ttu-id="9e972-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e972-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e972-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e972-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e972-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e972-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="9e972-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e972-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e972-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e972-114">Not supported.</span></span> |
| <span data-ttu-id="9e972-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e972-115">Application</span></span>                            | <span data-ttu-id="9e972-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9e972-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e972-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e972-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9e972-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e972-118">Request headers</span></span>

| <span data-ttu-id="9e972-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9e972-119">Name</span></span>          | <span data-ttu-id="9e972-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e972-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9e972-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e972-121">Authorization</span></span> | <span data-ttu-id="9e972-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="9e972-122">Bearer {token}.</span></span> <span data-ttu-id="9e972-123">Required.</span><span class="sxs-lookup"><span data-stu-id="9e972-123">Required.</span></span> |
| <span data-ttu-id="9e972-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e972-124">Content-Type</span></span> | <span data-ttu-id="9e972-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="9e972-125">application/json.</span></span> <span data-ttu-id="9e972-126">Required.</span><span class="sxs-lookup"><span data-stu-id="9e972-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e972-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e972-127">Request body</span></span>

<span data-ttu-id="9e972-128">No corpo da solicitação, forneça o identificador do objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e972-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="9e972-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e972-129">Response</span></span>

<span data-ttu-id="9e972-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="9e972-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="9e972-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="9e972-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e972-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e972-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e972-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e972-133">Request</span></span>

<span data-ttu-id="9e972-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e972-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e972-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e972-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="9e972-136">C#</span><span class="sxs-lookup"><span data-stu-id="9e972-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e972-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e972-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e972-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e972-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e972-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e972-139">Response</span></span>

<span data-ttu-id="9e972-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e972-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
