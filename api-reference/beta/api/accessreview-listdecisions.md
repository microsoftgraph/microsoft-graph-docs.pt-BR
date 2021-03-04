---
title: Listar decisões do accessReview
description: No recurso de revisões de acesso do Azure AD, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b21a7ac3d10e324835922544232a10fbcade409c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439344"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="51f0c-103">Listar decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-103">List accessReview decisions</span></span>

<span data-ttu-id="51f0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51f0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f0c-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) recupere as decisões de um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="51f0c-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="51f0c-106">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="51f0c-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="51f0c-107">Em vez disso, o chamador deve navegar pela relação para encontrar um objeto para `instance` uma instância atual ou anterior da revisão de `accessReview` acesso.</span><span class="sxs-lookup"><span data-stu-id="51f0c-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="51f0c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="51f0c-108">Permissions</span></span>
<span data-ttu-id="51f0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51f0c-111">Permission type</span></span>                        | <span data-ttu-id="51f0c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51f0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="51f0c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51f0c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="51f0c-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51f0c-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="51f0c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51f0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51f0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51f0c-116">Not supported.</span></span> |
|<span data-ttu-id="51f0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51f0c-117">Application</span></span>                            | <span data-ttu-id="51f0c-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="51f0c-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="51f0c-119">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="51f0c-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="51f0c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51f0c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="51f0c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51f0c-121">Request headers</span></span>
| <span data-ttu-id="51f0c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="51f0c-122">Name</span></span>         | <span data-ttu-id="51f0c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f0c-123">Type</span></span>        | <span data-ttu-id="51f0c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f0c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="51f0c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="51f0c-125">Authorization</span></span> | <span data-ttu-id="51f0c-126">string</span><span class="sxs-lookup"><span data-stu-id="51f0c-126">string</span></span> | <span data-ttu-id="51f0c-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51f0c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51f0c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51f0c-129">Request body</span></span>
<span data-ttu-id="51f0c-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="51f0c-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="51f0c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f0c-131">Response</span></span>
<span data-ttu-id="51f0c-132">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200, OK` [objetos accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51f0c-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51f0c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51f0c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51f0c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51f0c-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51f0c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="51f0c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="51f0c-136">C#</span><span class="sxs-lookup"><span data-stu-id="51f0c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51f0c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51f0c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51f0c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51f0c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51f0c-139">Java</span><span class="sxs-lookup"><span data-stu-id="51f0c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51f0c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="51f0c-140">Response</span></span>
><span data-ttu-id="51f0c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51f0c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="51f0c-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="51f0c-143">See also</span></span>

| <span data-ttu-id="51f0c-144">Método</span><span class="sxs-lookup"><span data-stu-id="51f0c-144">Method</span></span>           | <span data-ttu-id="51f0c-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51f0c-145">Return Type</span></span>    |<span data-ttu-id="51f0c-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f0c-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51f0c-147">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-147">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="51f0c-148">accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="51f0c-149">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="51f0c-149">Retrieve an access review.</span></span> |
|[<span data-ttu-id="51f0c-150">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-150">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="51f0c-151">[Coleção accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="51f0c-151">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="51f0c-152">Como revisor, receba minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="51f0c-152">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="51f0c-153">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-153">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="51f0c-154">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51f0c-154">None.</span></span>   |   <span data-ttu-id="51f0c-155">Envie um lembrete aos revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="51f0c-155">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="51f0c-156">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-156">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="51f0c-157">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51f0c-157">None.</span></span>   |   <span data-ttu-id="51f0c-158">Pare um accessReview.</span><span class="sxs-lookup"><span data-stu-id="51f0c-158">Stop an accessReview.</span></span> |
|[<span data-ttu-id="51f0c-159">Redefinir as decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-159">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="51f0c-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51f0c-160">None.</span></span>   |   <span data-ttu-id="51f0c-161">Redefinir as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="51f0c-161">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="51f0c-162">Aplicar decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="51f0c-162">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="51f0c-163">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51f0c-163">None.</span></span>   |   <span data-ttu-id="51f0c-164">Aplicar as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="51f0c-164">Apply the decisions from a completed accessReview.</span></span>|


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


