---
title: Remover revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 215f675f6fa4dd9461f7e36c26c135face9b95d9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172729"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="eabf3-105">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="eabf3-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eabf3-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="eabf3-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="eabf3-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="eabf3-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="eabf3-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="eabf3-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="eabf3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eabf3-109">Permissions</span></span>
<span data-ttu-id="eabf3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eabf3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eabf3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eabf3-112">Permission type</span></span>                        | <span data-ttu-id="eabf3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eabf3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eabf3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eabf3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="eabf3-115">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eabf3-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="eabf3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eabf3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eabf3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eabf3-117">Not supported.</span></span> |
|<span data-ttu-id="eabf3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eabf3-118">Application</span></span>                            | <span data-ttu-id="eabf3-119">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="eabf3-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="eabf3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eabf3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="eabf3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eabf3-121">Request headers</span></span>
| <span data-ttu-id="eabf3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="eabf3-122">Name</span></span>         | <span data-ttu-id="eabf3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="eabf3-123">Type</span></span>        | <span data-ttu-id="eabf3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eabf3-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eabf3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eabf3-125">Authorization</span></span> | <span data-ttu-id="eabf3-126">string</span><span class="sxs-lookup"><span data-stu-id="eabf3-126">string</span></span> | <span data-ttu-id="eabf3-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eabf3-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eabf3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eabf3-129">Request body</span></span>
<span data-ttu-id="eabf3-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="eabf3-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="eabf3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eabf3-131">Response</span></span>
<span data-ttu-id="eabf3-132">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="eabf3-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="eabf3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eabf3-133">Example</span></span>

<span data-ttu-id="eabf3-134">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="eabf3-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="eabf3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eabf3-135">Request</span></span>
<span data-ttu-id="eabf3-136">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="eabf3-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eabf3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="eabf3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eabf3-138">C#</span><span class="sxs-lookup"><span data-stu-id="eabf3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eabf3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="eabf3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eabf3-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eabf3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eabf3-141">Java</span><span class="sxs-lookup"><span data-stu-id="eabf3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eabf3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eabf3-142">Response</span></span>
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
