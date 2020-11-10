---
title: Remover revisor accessReview
description: Remover um revisor de revisão do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3efa60e8b92c47a60d6782a22146c7a63f6ba0f9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951494"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="b3fe8-103">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="b3fe8-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="b3fe8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fe8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3fe8-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="b3fe8-106">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="b3fe8-107">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="b3fe8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3fe8-108">Permissions</span></span>
<span data-ttu-id="b3fe8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3fe8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3fe8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3fe8-111">Permission type</span></span>                        | <span data-ttu-id="b3fe8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3fe8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3fe8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3fe8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3fe8-114">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b3fe8-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b3fe8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3fe8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3fe8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-116">Not supported.</span></span> |
|<span data-ttu-id="b3fe8-117">Application</span><span class="sxs-lookup"><span data-stu-id="b3fe8-117">Application</span></span>                            | <span data-ttu-id="b3fe8-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="b3fe8-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3fe8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3fe8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="b3fe8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fe8-120">Request headers</span></span>
| <span data-ttu-id="b3fe8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b3fe8-121">Name</span></span>         | <span data-ttu-id="b3fe8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3fe8-122">Type</span></span>        | <span data-ttu-id="b3fe8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fe8-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b3fe8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3fe8-124">Authorization</span></span> | <span data-ttu-id="b3fe8-125">string</span><span class="sxs-lookup"><span data-stu-id="b3fe8-125">string</span></span> | <span data-ttu-id="b3fe8-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3fe8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fe8-128">Request body</span></span>
<span data-ttu-id="b3fe8-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="b3fe8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fe8-130">Response</span></span>
<span data-ttu-id="b3fe8-131">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-131">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3fe8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3fe8-132">Example</span></span>

<span data-ttu-id="b3fe8-133">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="b3fe8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fe8-134">Request</span></span>
<span data-ttu-id="b3fe8-135">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="b3fe8-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="b3fe8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3fe8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="b3fe8-137">C#</span><span class="sxs-lookup"><span data-stu-id="b3fe8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3fe8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3fe8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3fe8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3fe8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3fe8-140">Java</span><span class="sxs-lookup"><span data-stu-id="b3fe8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b3fe8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fe8-141">Response</span></span>
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


