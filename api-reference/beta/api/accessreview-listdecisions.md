---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef1db408a4b47928e86f47f30588a8e09f98dad7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586198"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="a12e9-103">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12e9-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a12e9-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a12e9-105">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="a12e9-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="a12e9-106">Em vez disso, o chamador deve `instance` navegar na relação para `accessReview` localizar um objeto para uma instância atual ou passada da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a12e9-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="a12e9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a12e9-107">Permissions</span></span>
<span data-ttu-id="a12e9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a12e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a12e9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a12e9-110">Permission type</span></span>                        | <span data-ttu-id="a12e9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a12e9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a12e9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a12e9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a12e9-113">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a12e9-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="a12e9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a12e9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a12e9-115">Not supported.</span></span> |
|<span data-ttu-id="a12e9-116">Application</span><span class="sxs-lookup"><span data-stu-id="a12e9-116">Application</span></span>                            | <span data-ttu-id="a12e9-117">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="a12e9-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="a12e9-118">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a12e9-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="a12e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a12e9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="a12e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a12e9-120">Request headers</span></span>
| <span data-ttu-id="a12e9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a12e9-121">Name</span></span>         | <span data-ttu-id="a12e9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a12e9-122">Type</span></span>        | <span data-ttu-id="a12e9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a12e9-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a12e9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a12e9-124">Authorization</span></span> | <span data-ttu-id="a12e9-125">string</span><span class="sxs-lookup"><span data-stu-id="a12e9-125">string</span></span> | <span data-ttu-id="a12e9-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a12e9-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a12e9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a12e9-128">Request body</span></span>
<span data-ttu-id="a12e9-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="a12e9-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="a12e9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a12e9-130">Response</span></span>
<span data-ttu-id="a12e9-131">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a12e9-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a12e9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a12e9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a12e9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a12e9-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="a12e9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a12e9-134">Response</span></span>
><span data-ttu-id="a12e9-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a12e9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a12e9-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a12e9-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a12e9-138">Basic</span><span class="sxs-lookup"><span data-stu-id="a12e9-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a12e9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a12e9-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="a12e9-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="a12e9-140">See also</span></span>

| <span data-ttu-id="a12e9-141">Método</span><span class="sxs-lookup"><span data-stu-id="a12e9-141">Method</span></span>           | <span data-ttu-id="a12e9-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a12e9-142">Return Type</span></span>    |<span data-ttu-id="a12e9-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a12e9-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a12e9-144">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="a12e9-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="a12e9-146">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a12e9-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="a12e9-147">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-147">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="a12e9-148">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="a12e9-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="a12e9-149">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a12e9-149">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a12e9-150">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-150">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="a12e9-151">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a12e9-151">None.</span></span>   |   <span data-ttu-id="a12e9-152">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a12e9-152">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a12e9-153">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-153">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="a12e9-154">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a12e9-154">None.</span></span>   |   <span data-ttu-id="a12e9-155">Parar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a12e9-155">Stop an accessReview.</span></span> |
|[<span data-ttu-id="a12e9-156">Redefinir decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-156">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="a12e9-157">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a12e9-157">None.</span></span>   |   <span data-ttu-id="a12e9-158">Redefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="a12e9-158">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="a12e9-159">Aplicar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="a12e9-159">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="a12e9-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a12e9-160">None.</span></span>   |   <span data-ttu-id="a12e9-161">Aplique as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="a12e9-161">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
