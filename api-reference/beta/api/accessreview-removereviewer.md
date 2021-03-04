---
title: Remover o revisor accessReview
description: Remover um revistor de revisão de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 83f136a3a9c131d5a05df92df2f3c3e3d3b6c75c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439294"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="c7300-103">Remover o revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="c7300-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="c7300-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7300-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7300-105">No recurso de revisões de acesso do Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como [revisor.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="c7300-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="c7300-106">Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e somente para uma revisão de acesso em que os revisadores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="c7300-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="c7300-107">Essa operação não é permitida para uma revisão de acesso na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão de acesso na qual os proprietários do grupo são atribuídos como revistores.</span><span class="sxs-lookup"><span data-stu-id="c7300-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="c7300-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7300-108">Permissions</span></span>
<span data-ttu-id="c7300-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7300-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7300-111">Permission type</span></span>                        | <span data-ttu-id="c7300-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7300-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7300-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7300-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7300-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7300-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c7300-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7300-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7300-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7300-116">Not supported.</span></span> |
|<span data-ttu-id="c7300-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7300-117">Application</span></span>                            | <span data-ttu-id="c7300-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="c7300-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7300-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7300-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="c7300-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7300-120">Request headers</span></span>
| <span data-ttu-id="c7300-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c7300-121">Name</span></span>         | <span data-ttu-id="c7300-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7300-122">Type</span></span>        | <span data-ttu-id="c7300-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7300-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c7300-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7300-124">Authorization</span></span> | <span data-ttu-id="c7300-125">string</span><span class="sxs-lookup"><span data-stu-id="c7300-125">string</span></span> | <span data-ttu-id="c7300-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7300-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7300-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7300-128">Request body</span></span>
<span data-ttu-id="c7300-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="c7300-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="c7300-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7300-130">Response</span></span>
<span data-ttu-id="c7300-131">Se tiver êxito, este método retornará um código de resposta de 200 séries.</span><span class="sxs-lookup"><span data-stu-id="c7300-131">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="c7300-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7300-132">Example</span></span>

<span data-ttu-id="c7300-133">Este é um exemplo de atualização de uma revisão de acesso única (não recorrente) para remover um revistor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="c7300-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="c7300-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7300-134">Request</span></span>
<span data-ttu-id="c7300-135">Na URL de solicitação, fornece a id do objeto accessReview e, em seguida, a id do objeto user.</span><span class="sxs-lookup"><span data-stu-id="c7300-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7300-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7300-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="c7300-137">C#</span><span class="sxs-lookup"><span data-stu-id="c7300-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7300-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7300-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7300-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7300-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7300-140">Java</span><span class="sxs-lookup"><span data-stu-id="c7300-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7300-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7300-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


