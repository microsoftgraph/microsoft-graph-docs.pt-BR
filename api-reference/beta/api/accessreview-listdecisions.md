---
title: Lista accessReview decisões
description: No Windows Azure AD para acessar o recurso de revisões, recuperar as decisões de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521793"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="17380-103">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="17380-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17380-104">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="17380-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="17380-105">Observe que uma análise mais acesso recorrente não terá um `decisions` relacionamento.</span><span class="sxs-lookup"><span data-stu-id="17380-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="17380-106">Em vez disso, o chamador deve navegar o `instance` relação para encontrar um `accessReview` objeto para uma instância atual ou passado da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="17380-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="17380-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="17380-107">Permissions</span></span>
<span data-ttu-id="17380-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17380-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17380-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17380-110">Permission type</span></span>                        | <span data-ttu-id="17380-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17380-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="17380-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17380-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="17380-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="17380-113"></span></span>  <span data-ttu-id="17380-114">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="17380-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="17380-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17380-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17380-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17380-116">Not supported.</span></span> |
|<span data-ttu-id="17380-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17380-117">Application</span></span>                            | <span data-ttu-id="17380-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17380-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17380-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17380-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="17380-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17380-120">Request headers</span></span>
| <span data-ttu-id="17380-121">Nome</span><span class="sxs-lookup"><span data-stu-id="17380-121">Name</span></span>         | <span data-ttu-id="17380-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="17380-122">Type</span></span>        | <span data-ttu-id="17380-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="17380-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="17380-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17380-124">Authorization</span></span> | <span data-ttu-id="17380-125">string</span><span class="sxs-lookup"><span data-stu-id="17380-125">string</span></span> | <span data-ttu-id="17380-126">Token de portador</span><span class="sxs-lookup"><span data-stu-id="17380-126">Bearer \{token\}.</span></span> <span data-ttu-id="17380-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17380-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17380-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17380-128">Request body</span></span>
<span data-ttu-id="17380-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="17380-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="17380-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="17380-130">Response</span></span>
<span data-ttu-id="17380-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17380-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17380-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17380-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17380-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17380-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="17380-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="17380-134">Response</span></span>
><span data-ttu-id="17380-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17380-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="17380-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="17380-137">See also</span></span>

| <span data-ttu-id="17380-138">Método</span><span class="sxs-lookup"><span data-stu-id="17380-138">Method</span></span>           | <span data-ttu-id="17380-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17380-139">Return Type</span></span>    |<span data-ttu-id="17380-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="17380-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17380-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="17380-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="17380-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="17380-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="17380-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="17380-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="17380-144">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="17380-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="17380-145">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="17380-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="17380-146">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="17380-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="17380-147">Enviar accessReview lembrete</span><span class="sxs-lookup"><span data-stu-id="17380-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="17380-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17380-148">None.</span></span>   |   <span data-ttu-id="17380-149">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="17380-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="17380-150">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="17380-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="17380-151">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17380-151">None.</span></span>   |   <span data-ttu-id="17380-152">Pare uma accessReview.</span><span class="sxs-lookup"><span data-stu-id="17380-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="17380-153">Redefinir accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="17380-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="17380-154">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17380-154">None.</span></span>   |   <span data-ttu-id="17380-155">Redefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="17380-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="17380-156">Aplicar accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="17380-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="17380-157">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="17380-157">None.</span></span>   |   <span data-ttu-id="17380-158">Aplique as decisões de um accessReview concluída.</span><span class="sxs-lookup"><span data-stu-id="17380-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
