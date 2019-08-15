---
title: Listar minhas decisões do accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview para o usuário de chamada como revisor.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b28c86b71d6b99826f2d54c389087c6d64e129f0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408801"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="06186-103">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="06186-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06186-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário de chamada como revisor.</span><span class="sxs-lookup"><span data-stu-id="06186-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="06186-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="06186-105">Permissions</span></span>
<span data-ttu-id="06186-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06186-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06186-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06186-108">Permission type</span></span>                        | <span data-ttu-id="06186-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06186-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="06186-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06186-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="06186-111">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="06186-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="06186-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06186-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06186-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06186-113">Not supported.</span></span> |
|<span data-ttu-id="06186-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06186-114">Application</span></span>                            | <span data-ttu-id="06186-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06186-115">Not supported.</span></span> |

<span data-ttu-id="06186-116">O usuário conectado também deve ter permissão para ler essa revisão de acesso específica.</span><span class="sxs-lookup"><span data-stu-id="06186-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="06186-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06186-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="06186-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06186-118">Request headers</span></span>
| <span data-ttu-id="06186-119">Nome</span><span class="sxs-lookup"><span data-stu-id="06186-119">Name</span></span>         | <span data-ttu-id="06186-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="06186-120">Type</span></span>        | <span data-ttu-id="06186-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="06186-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="06186-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06186-122">Authorization</span></span> | <span data-ttu-id="06186-123">string</span><span class="sxs-lookup"><span data-stu-id="06186-123">string</span></span> | <span data-ttu-id="06186-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06186-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06186-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06186-126">Request body</span></span>
<span data-ttu-id="06186-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="06186-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="06186-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="06186-128">Response</span></span>
<span data-ttu-id="06186-129">Se bem-sucedido, este método retorna um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="06186-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="06186-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06186-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06186-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06186-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="06186-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="06186-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06186-133">C#</span><span class="sxs-lookup"><span data-stu-id="06186-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06186-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06186-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06186-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="06186-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="06186-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="06186-136">Response</span></span>
><span data-ttu-id="06186-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06186-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="06186-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="06186-139">See also</span></span>

| <span data-ttu-id="06186-140">Método</span><span class="sxs-lookup"><span data-stu-id="06186-140">Method</span></span>           | <span data-ttu-id="06186-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06186-141">Return Type</span></span>    |<span data-ttu-id="06186-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="06186-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06186-143">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="06186-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="06186-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="06186-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="06186-145">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="06186-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="06186-146">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="06186-146">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="06186-147">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="06186-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="06186-148">Recuperar todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="06186-148">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
