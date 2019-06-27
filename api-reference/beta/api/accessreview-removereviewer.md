---
title: Remover revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c83c8be63446c347c19b479deb6e72f171a91ce1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258839"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="da2be-105">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="da2be-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da2be-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="da2be-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="da2be-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="da2be-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="da2be-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="da2be-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="da2be-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="da2be-109">Permissions</span></span>
<span data-ttu-id="da2be-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2be-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da2be-112">Permission type</span></span>                        | <span data-ttu-id="da2be-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da2be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2be-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da2be-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="da2be-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2be-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="da2be-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da2be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da2be-117">Not supported.</span></span> |
|<span data-ttu-id="da2be-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da2be-118">Application</span></span>                            | <span data-ttu-id="da2be-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da2be-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2be-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da2be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="da2be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da2be-121">Request headers</span></span>
| <span data-ttu-id="da2be-122">Nome</span><span class="sxs-lookup"><span data-stu-id="da2be-122">Name</span></span>         | <span data-ttu-id="da2be-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="da2be-123">Type</span></span>        | <span data-ttu-id="da2be-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="da2be-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="da2be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da2be-125">Authorization</span></span> | <span data-ttu-id="da2be-126">string</span><span class="sxs-lookup"><span data-stu-id="da2be-126">string</span></span> | <span data-ttu-id="da2be-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da2be-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da2be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da2be-129">Request body</span></span>
<span data-ttu-id="da2be-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="da2be-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="da2be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da2be-131">Response</span></span>
<span data-ttu-id="da2be-132">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="da2be-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="da2be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da2be-133">Example</span></span>

<span data-ttu-id="da2be-134">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="da2be-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="da2be-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da2be-135">Request</span></span>
<span data-ttu-id="da2be-136">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="da2be-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```

##### <a name="response"></a><span data-ttu-id="da2be-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="da2be-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="da2be-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="da2be-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da2be-139">C#</span><span class="sxs-lookup"><span data-stu-id="da2be-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da2be-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="da2be-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="da2be-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da2be-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_accessReview_reviewer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
