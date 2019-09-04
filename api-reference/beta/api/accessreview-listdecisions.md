---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6df2b0067fdf939933a7f9849f8b358fbd69ed3a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719290"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="f533a-103">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f533a-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="f533a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="f533a-105">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="f533a-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="f533a-106">Em vez disso, o chamador deve `instance` navegar na relação para `accessReview` localizar um objeto para uma instância atual ou passada da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f533a-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="f533a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f533a-107">Permissions</span></span>
<span data-ttu-id="f533a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f533a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f533a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f533a-110">Permission type</span></span>                        | <span data-ttu-id="f533a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f533a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f533a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f533a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f533a-113">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f533a-113">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f533a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f533a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f533a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f533a-115">Not supported.</span></span> |
|<span data-ttu-id="f533a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f533a-116">Application</span></span>                            | <span data-ttu-id="f533a-117">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="f533a-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="f533a-118">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f533a-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f533a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f533a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="f533a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f533a-120">Request headers</span></span>
| <span data-ttu-id="f533a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f533a-121">Name</span></span>         | <span data-ttu-id="f533a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f533a-122">Type</span></span>        | <span data-ttu-id="f533a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f533a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f533a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f533a-124">Authorization</span></span> | <span data-ttu-id="f533a-125">string</span><span class="sxs-lookup"><span data-stu-id="f533a-125">string</span></span> | <span data-ttu-id="f533a-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f533a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f533a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f533a-128">Request body</span></span>
<span data-ttu-id="f533a-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="f533a-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f533a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f533a-130">Response</span></span>
<span data-ttu-id="f533a-131">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f533a-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f533a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f533a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f533a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f533a-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f533a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f533a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f533a-135">C#</span><span class="sxs-lookup"><span data-stu-id="f533a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f533a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f533a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f533a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f533a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f533a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f533a-138">Response</span></span>
><span data-ttu-id="f533a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f533a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f533a-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="f533a-141">See also</span></span>

| <span data-ttu-id="f533a-142">Método</span><span class="sxs-lookup"><span data-stu-id="f533a-142">Method</span></span>           | <span data-ttu-id="f533a-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f533a-143">Return Type</span></span>    |<span data-ttu-id="f533a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="f533a-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f533a-145">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="f533a-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f533a-147">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f533a-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="f533a-148">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-148">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="f533a-149">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="f533a-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="f533a-150">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="f533a-150">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="f533a-151">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-151">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="f533a-152">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f533a-152">None.</span></span>   |   <span data-ttu-id="f533a-153">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="f533a-153">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="f533a-154">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-154">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="f533a-155">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f533a-155">None.</span></span>   |   <span data-ttu-id="f533a-156">Parar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="f533a-156">Stop an accessReview.</span></span> |
|[<span data-ttu-id="f533a-157">Redefinir decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-157">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="f533a-158">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f533a-158">None.</span></span>   |   <span data-ttu-id="f533a-159">Redefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="f533a-159">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="f533a-160">Aplicar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="f533a-160">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="f533a-161">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f533a-161">None.</span></span>   |   <span data-ttu-id="f533a-162">Aplique as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="f533a-162">Apply the decisions from a completed accessReview.</span></span>|


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
