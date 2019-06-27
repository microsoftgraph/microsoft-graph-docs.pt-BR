---
title: Listar minhas decisões do accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview para o usuário de chamada como revisor.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b506ab17abe270bfd3ecc27ab70f7699487528a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258846"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="10f0c-103">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="10f0c-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10f0c-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário de chamada como revisor.</span><span class="sxs-lookup"><span data-stu-id="10f0c-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="10f0c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="10f0c-105">Permissions</span></span>
<span data-ttu-id="10f0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f0c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10f0c-108">Permission type</span></span>                        | <span data-ttu-id="10f0c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10f0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10f0c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10f0c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="10f0c-111">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="10f0c-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="10f0c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10f0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10f0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f0c-113">Not supported.</span></span> |
|<span data-ttu-id="10f0c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10f0c-114">Application</span></span>                            | <span data-ttu-id="10f0c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f0c-115">Not supported.</span></span> |

<span data-ttu-id="10f0c-116">O usuário conectado também deve ter permissão para ler essa revisão de acesso específica.</span><span class="sxs-lookup"><span data-stu-id="10f0c-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="10f0c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10f0c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="10f0c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10f0c-118">Request headers</span></span>
| <span data-ttu-id="10f0c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="10f0c-119">Name</span></span>         | <span data-ttu-id="10f0c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="10f0c-120">Type</span></span>        | <span data-ttu-id="10f0c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f0c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="10f0c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10f0c-122">Authorization</span></span> | <span data-ttu-id="10f0c-123">string</span><span class="sxs-lookup"><span data-stu-id="10f0c-123">string</span></span> | <span data-ttu-id="10f0c-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10f0c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10f0c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10f0c-126">Request body</span></span>
<span data-ttu-id="10f0c-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="10f0c-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="10f0c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f0c-128">Response</span></span>
<span data-ttu-id="10f0c-129">Se bem-sucedido, este método retorna um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="10f0c-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="10f0c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10f0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10f0c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10f0c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="10f0c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f0c-132">Response</span></span>
><span data-ttu-id="10f0c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10f0c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="10f0c-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="10f0c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10f0c-136">C#</span><span class="sxs-lookup"><span data-stu-id="10f0c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10f0c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="10f0c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="10f0c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="10f0c-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="10f0c-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="10f0c-139">See also</span></span>

| <span data-ttu-id="10f0c-140">Método</span><span class="sxs-lookup"><span data-stu-id="10f0c-140">Method</span></span>           | <span data-ttu-id="10f0c-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10f0c-141">Return Type</span></span>    |<span data-ttu-id="10f0c-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f0c-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10f0c-143">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="10f0c-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="10f0c-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="10f0c-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="10f0c-145">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="10f0c-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="10f0c-146">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="10f0c-146">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="10f0c-147">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="10f0c-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="10f0c-148">Recuperar todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="10f0c-148">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
