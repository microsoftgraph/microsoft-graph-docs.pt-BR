---
title: Remover revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e2034023c6f8b842ff74aa82ddb42a482c939cc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408776"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="64fb8-105">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="64fb8-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64fb8-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="64fb8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="64fb8-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="64fb8-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="64fb8-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="64fb8-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="64fb8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="64fb8-109">Permissions</span></span>
<span data-ttu-id="64fb8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fb8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64fb8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64fb8-112">Permission type</span></span>                        | <span data-ttu-id="64fb8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64fb8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="64fb8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64fb8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="64fb8-115">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64fb8-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="64fb8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64fb8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fb8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64fb8-117">Not supported.</span></span> |
|<span data-ttu-id="64fb8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64fb8-118">Application</span></span>                            | <span data-ttu-id="64fb8-119">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="64fb8-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="64fb8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="64fb8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb8-121">Request headers</span></span>
| <span data-ttu-id="64fb8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="64fb8-122">Name</span></span>         | <span data-ttu-id="64fb8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="64fb8-123">Type</span></span>        | <span data-ttu-id="64fb8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="64fb8-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="64fb8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64fb8-125">Authorization</span></span> | <span data-ttu-id="64fb8-126">string</span><span class="sxs-lookup"><span data-stu-id="64fb8-126">string</span></span> | <span data-ttu-id="64fb8-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64fb8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64fb8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb8-129">Request body</span></span>
<span data-ttu-id="64fb8-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="64fb8-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="64fb8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb8-131">Response</span></span>
<span data-ttu-id="64fb8-132">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="64fb8-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="64fb8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64fb8-133">Example</span></span>

<span data-ttu-id="64fb8-134">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="64fb8-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="64fb8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb8-135">Request</span></span>
<span data-ttu-id="64fb8-136">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="64fb8-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64fb8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64fb8-138">C#</span><span class="sxs-lookup"><span data-stu-id="64fb8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64fb8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64fb8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64fb8-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64fb8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64fb8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb8-141">Response</span></span>
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
