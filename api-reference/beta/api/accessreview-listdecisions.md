---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cfb41a948264ef846638395732fe61c3e51f5008
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983573"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="bf75d-103">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-103">List accessReview decisions</span></span>

<span data-ttu-id="bf75d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf75d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf75d-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="bf75d-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="bf75d-106">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="bf75d-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="bf75d-107">Em vez disso, o chamador deve navegar na `instance` relação para localizar um `accessReview` objeto para uma instância atual ou passada da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bf75d-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf75d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf75d-108">Permissions</span></span>
<span data-ttu-id="bf75d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf75d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf75d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf75d-111">Permission type</span></span>                        | <span data-ttu-id="bf75d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf75d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf75d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf75d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf75d-114">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bf75d-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="bf75d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf75d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf75d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf75d-116">Not supported.</span></span> |
|<span data-ttu-id="bf75d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf75d-117">Application</span></span>                            | <span data-ttu-id="bf75d-118">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="bf75d-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="bf75d-119">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bf75d-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf75d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf75d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="bf75d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf75d-121">Request headers</span></span>
| <span data-ttu-id="bf75d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bf75d-122">Name</span></span>         | <span data-ttu-id="bf75d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf75d-123">Type</span></span>        | <span data-ttu-id="bf75d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf75d-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bf75d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf75d-125">Authorization</span></span> | <span data-ttu-id="bf75d-126">string</span><span class="sxs-lookup"><span data-stu-id="bf75d-126">string</span></span> | <span data-ttu-id="bf75d-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf75d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf75d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf75d-129">Request body</span></span>
<span data-ttu-id="bf75d-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="bf75d-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bf75d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf75d-131">Response</span></span>
<span data-ttu-id="bf75d-132">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf75d-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf75d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf75d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf75d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf75d-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf75d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf75d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="bf75d-136">C#</span><span class="sxs-lookup"><span data-stu-id="bf75d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf75d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf75d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf75d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf75d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bf75d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf75d-139">Response</span></span>
><span data-ttu-id="bf75d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf75d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bf75d-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf75d-142">See also</span></span>

| <span data-ttu-id="bf75d-143">Método</span><span class="sxs-lookup"><span data-stu-id="bf75d-143">Method</span></span>           | <span data-ttu-id="bf75d-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bf75d-144">Return Type</span></span>    |<span data-ttu-id="bf75d-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf75d-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf75d-146">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="bf75d-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="bf75d-148">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bf75d-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="bf75d-149">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="bf75d-150">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="bf75d-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="bf75d-151">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="bf75d-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="bf75d-152">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="bf75d-153">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf75d-153">None.</span></span>   |   <span data-ttu-id="bf75d-154">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="bf75d-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="bf75d-155">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="bf75d-156">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf75d-156">None.</span></span>   |   <span data-ttu-id="bf75d-157">Parar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="bf75d-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="bf75d-158">Redefinir decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="bf75d-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf75d-159">None.</span></span>   |   <span data-ttu-id="bf75d-160">Redefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="bf75d-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="bf75d-161">Aplicar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="bf75d-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="bf75d-162">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf75d-162">None.</span></span>   |   <span data-ttu-id="bf75d-163">Aplique as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="bf75d-163">Apply the decisions from a completed accessReview.</span></span>|


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


