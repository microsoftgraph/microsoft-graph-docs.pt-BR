---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 123eeb46ba38937722e68bee6aaa001c86320106
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299637"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="efaef-103">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efaef-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="efaef-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="efaef-105">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="efaef-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="efaef-106">Em vez disso, o chamador deve `instance` navegar na relação para `accessReview` localizar um objeto para uma instância atual ou passada da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="efaef-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="efaef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="efaef-107">Permissions</span></span>
<span data-ttu-id="efaef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efaef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efaef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efaef-110">Permission type</span></span>                        | <span data-ttu-id="efaef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efaef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="efaef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efaef-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="efaef-113">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="efaef-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="efaef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efaef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efaef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efaef-115">Not supported.</span></span> |
|<span data-ttu-id="efaef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efaef-116">Application</span></span>                            | <span data-ttu-id="efaef-117">AccessReview. Read. All</span><span class="sxs-lookup"><span data-stu-id="efaef-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="efaef-118">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="efaef-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="efaef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efaef-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="efaef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efaef-120">Request headers</span></span>
| <span data-ttu-id="efaef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="efaef-121">Name</span></span>         | <span data-ttu-id="efaef-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="efaef-122">Type</span></span>        | <span data-ttu-id="efaef-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="efaef-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="efaef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="efaef-124">Authorization</span></span> | <span data-ttu-id="efaef-125">string</span><span class="sxs-lookup"><span data-stu-id="efaef-125">string</span></span> | <span data-ttu-id="efaef-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efaef-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efaef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efaef-128">Request body</span></span>
<span data-ttu-id="efaef-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="efaef-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="efaef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="efaef-130">Response</span></span>
<span data-ttu-id="efaef-131">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efaef-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efaef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efaef-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efaef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efaef-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="efaef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="efaef-134">Response</span></span>
><span data-ttu-id="efaef-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efaef-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="efaef-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="efaef-137">See also</span></span>

| <span data-ttu-id="efaef-138">Método</span><span class="sxs-lookup"><span data-stu-id="efaef-138">Method</span></span>           | <span data-ttu-id="efaef-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="efaef-139">Return Type</span></span>    |<span data-ttu-id="efaef-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="efaef-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efaef-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="efaef-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="efaef-143">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="efaef-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="efaef-144">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="efaef-145">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="efaef-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="efaef-146">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="efaef-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="efaef-147">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="efaef-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efaef-148">None.</span></span>   |   <span data-ttu-id="efaef-149">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="efaef-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="efaef-150">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="efaef-151">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efaef-151">None.</span></span>   |   <span data-ttu-id="efaef-152">Parar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="efaef-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="efaef-153">Redefinir decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="efaef-154">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efaef-154">None.</span></span>   |   <span data-ttu-id="efaef-155">ReDefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="efaef-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="efaef-156">Aplicar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="efaef-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="efaef-157">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="efaef-157">None.</span></span>   |   <span data-ttu-id="efaef-158">Aplique as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="efaef-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
