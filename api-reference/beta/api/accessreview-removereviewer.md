---
title: Remover revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f81f7b4befc99ad457d570e5e66a2ce97bfe4ce2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441869"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="d26d7-105">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="d26d7-105">Remove accessReview reviewer</span></span>

<span data-ttu-id="d26d7-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d26d7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d26d7-107">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="d26d7-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="d26d7-108">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="d26d7-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="d26d7-109">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="d26d7-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d26d7-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d26d7-110">Permissions</span></span>
<span data-ttu-id="d26d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d26d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d26d7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d26d7-113">Permission type</span></span>                        | <span data-ttu-id="d26d7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d26d7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d26d7-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d26d7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d26d7-116">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d26d7-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d26d7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d26d7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d26d7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d26d7-118">Not supported.</span></span> |
|<span data-ttu-id="d26d7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d26d7-119">Application</span></span>                            | <span data-ttu-id="d26d7-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="d26d7-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="d26d7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d26d7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="d26d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d26d7-122">Request headers</span></span>
| <span data-ttu-id="d26d7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d26d7-123">Name</span></span>         | <span data-ttu-id="d26d7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d26d7-124">Type</span></span>        | <span data-ttu-id="d26d7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d26d7-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d26d7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d26d7-126">Authorization</span></span> | <span data-ttu-id="d26d7-127">string</span><span class="sxs-lookup"><span data-stu-id="d26d7-127">string</span></span> | <span data-ttu-id="d26d7-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d26d7-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d26d7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d26d7-130">Request body</span></span>
<span data-ttu-id="d26d7-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d26d7-131">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="d26d7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26d7-132">Response</span></span>
<span data-ttu-id="d26d7-133">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="d26d7-133">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="d26d7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d26d7-134">Example</span></span>

<span data-ttu-id="d26d7-135">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="d26d7-135">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="d26d7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d26d7-136">Request</span></span>
<span data-ttu-id="d26d7-137">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="d26d7-137">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="d26d7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d26d7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="d26d7-139">C#</span><span class="sxs-lookup"><span data-stu-id="d26d7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d26d7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d26d7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d26d7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d26d7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d26d7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d26d7-142">Response</span></span>
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
