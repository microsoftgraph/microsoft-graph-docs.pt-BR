---
title: Listar minhas decisões do accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview para o usuário de chamada como revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7722d6084399fc00b0f99932ac7173b2d83dfa08
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123570"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="5d7d6-103">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="5d7d6-103">List my accessReview decisions</span></span>

<span data-ttu-id="5d7d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d7d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d7d6-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário de chamada como revisor.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d7d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d7d6-106">Permissions</span></span>
<span data-ttu-id="5d7d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d7d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d7d6-109">Permission type</span></span>                        | <span data-ttu-id="5d7d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d7d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d7d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d7d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d7d6-112">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5d7d6-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="5d7d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d7d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-114">Not supported.</span></span> |
|<span data-ttu-id="5d7d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d7d6-115">Application</span></span>                            | <span data-ttu-id="5d7d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-116">Not supported.</span></span> |

<span data-ttu-id="5d7d6-117">O usuário conectado também deve ter permissão para ler essa revisão de acesso específica.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="5d7d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d7d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="5d7d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7d6-119">Request headers</span></span>
| <span data-ttu-id="5d7d6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5d7d6-120">Name</span></span>         | <span data-ttu-id="5d7d6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d7d6-121">Type</span></span>        | <span data-ttu-id="5d7d6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7d6-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5d7d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d7d6-123">Authorization</span></span> | <span data-ttu-id="5d7d6-124">string</span><span class="sxs-lookup"><span data-stu-id="5d7d6-124">string</span></span> | <span data-ttu-id="5d7d6-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d7d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7d6-127">Request body</span></span>
<span data-ttu-id="5d7d6-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5d7d6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d7d6-129">Response</span></span>
<span data-ttu-id="5d7d6-130">Se bem-sucedido, este método retorna um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="5d7d6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d7d6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d7d6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d7d6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5d7d6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d7d6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="5d7d6-134">C#</span><span class="sxs-lookup"><span data-stu-id="5d7d6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d7d6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d7d6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d7d6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d7d6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d7d6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d7d6-137">Response</span></span>
><span data-ttu-id="5d7d6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5d7d6-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="5d7d6-140">See also</span></span>

| <span data-ttu-id="5d7d6-141">Método</span><span class="sxs-lookup"><span data-stu-id="5d7d6-141">Method</span></span>           | <span data-ttu-id="5d7d6-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d7d6-142">Return Type</span></span>    |<span data-ttu-id="5d7d6-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7d6-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5d7d6-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="5d7d6-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="5d7d6-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="5d7d6-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="5d7d6-146">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="5d7d6-147">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="5d7d6-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="5d7d6-148">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="5d7d6-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="5d7d6-149">Recuperar todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="5d7d6-149">Retrieve all the decisions of an accessReview.</span></span>|


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
