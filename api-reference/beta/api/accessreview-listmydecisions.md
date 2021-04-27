---
title: Listar minhas decisões do accessReview
description: No recurso de revisões de acesso do Azure AD, recupere as decisões de um objeto accessReview para o usuário chamador como revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 31f065033d1980c8a1ab640294f52f893a1f02f0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048467"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="d687a-103">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="d687a-103">List my accessReview decisions</span></span>

<span data-ttu-id="d687a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d687a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d687a-105">No recurso de revisões de acesso do Azure AD, recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário chamador como [revisor.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="d687a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="d687a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d687a-106">Permissions</span></span>
<span data-ttu-id="d687a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d687a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d687a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d687a-109">Permission type</span></span>                        | <span data-ttu-id="d687a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d687a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d687a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d687a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d687a-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d687a-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="d687a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d687a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d687a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d687a-114">Not supported.</span></span> |
|<span data-ttu-id="d687a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d687a-115">Application</span></span>                            | <span data-ttu-id="d687a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d687a-116">Not supported.</span></span> |

<span data-ttu-id="d687a-117">O usuário inscreveu também deve ter permissão para ler essa revisão de acesso específica.</span><span class="sxs-lookup"><span data-stu-id="d687a-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d687a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d687a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="d687a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d687a-119">Request headers</span></span>
| <span data-ttu-id="d687a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d687a-120">Name</span></span>         | <span data-ttu-id="d687a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d687a-121">Type</span></span>        | <span data-ttu-id="d687a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d687a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d687a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d687a-123">Authorization</span></span> | <span data-ttu-id="d687a-124">string</span><span class="sxs-lookup"><span data-stu-id="d687a-124">string</span></span> | <span data-ttu-id="d687a-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d687a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d687a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d687a-127">Request body</span></span>
<span data-ttu-id="d687a-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d687a-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d687a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d687a-129">Response</span></span>
<span data-ttu-id="d687a-130">Se tiver êxito, este método retornará um código de resposta e uma matriz de objetos `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="d687a-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="d687a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d687a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d687a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d687a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d687a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d687a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="d687a-134">C#</span><span class="sxs-lookup"><span data-stu-id="d687a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d687a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d687a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d687a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d687a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d687a-137">Java</span><span class="sxs-lookup"><span data-stu-id="d687a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d687a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d687a-138">Response</span></span>
><span data-ttu-id="d687a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d687a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d687a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="d687a-140">See also</span></span>

| <span data-ttu-id="d687a-141">Método</span><span class="sxs-lookup"><span data-stu-id="d687a-141">Method</span></span>           | <span data-ttu-id="d687a-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d687a-142">Return Type</span></span>    |<span data-ttu-id="d687a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d687a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d687a-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="d687a-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d687a-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="d687a-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d687a-146">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d687a-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d687a-147">Listar decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="d687a-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d687a-148">[Coleção accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="d687a-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d687a-149">Recupere todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d687a-149">Retrieve all the decisions of an accessReview.</span></span>|


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


