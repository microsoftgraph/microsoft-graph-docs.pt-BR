---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459625"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="96e94-103">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e94-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="96e94-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="96e94-105">Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.</span><span class="sxs-lookup"><span data-stu-id="96e94-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="96e94-106">Em vez disso, o chamador deve `instance` navegar na relação para `accessReview` localizar um objeto para uma instância atual ou passada da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="96e94-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="96e94-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="96e94-107">Permissions</span></span>
<span data-ttu-id="96e94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96e94-110">Permission type</span></span>                        | <span data-ttu-id="96e94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96e94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="96e94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96e94-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="96e94-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="96e94-113"></span></span>  <span data-ttu-id="96e94-114">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="96e94-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="96e94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96e94-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96e94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e94-116">Not supported.</span></span> |
|<span data-ttu-id="96e94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96e94-117">Application</span></span>                            | <span data-ttu-id="96e94-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e94-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96e94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96e94-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="96e94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96e94-120">Request headers</span></span>
| <span data-ttu-id="96e94-121">Nome</span><span class="sxs-lookup"><span data-stu-id="96e94-121">Name</span></span>         | <span data-ttu-id="96e94-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="96e94-122">Type</span></span>        | <span data-ttu-id="96e94-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="96e94-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="96e94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="96e94-124">Authorization</span></span> | <span data-ttu-id="96e94-125">string</span><span class="sxs-lookup"><span data-stu-id="96e94-125">string</span></span> | <span data-ttu-id="96e94-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96e94-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96e94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96e94-128">Request body</span></span>
<span data-ttu-id="96e94-129">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="96e94-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="96e94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e94-130">Response</span></span>
<span data-ttu-id="96e94-131">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96e94-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e94-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96e94-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96e94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96e94-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="96e94-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e94-134">Response</span></span>
><span data-ttu-id="96e94-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96e94-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="96e94-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="96e94-137">See also</span></span>

| <span data-ttu-id="96e94-138">Método</span><span class="sxs-lookup"><span data-stu-id="96e94-138">Method</span></span>           | <span data-ttu-id="96e94-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96e94-139">Return Type</span></span>    |<span data-ttu-id="96e94-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="96e94-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96e94-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="96e94-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="96e94-143">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="96e94-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="96e94-144">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="96e94-145">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="96e94-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="96e94-146">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="96e94-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="96e94-147">Enviar lembrete accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="96e94-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96e94-148">None.</span></span>   |   <span data-ttu-id="96e94-149">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="96e94-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="96e94-150">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="96e94-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96e94-151">None.</span></span>   |   <span data-ttu-id="96e94-152">Parar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="96e94-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="96e94-153">Redefinir decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="96e94-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96e94-154">None.</span></span>   |   <span data-ttu-id="96e94-155">ReDefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="96e94-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="96e94-156">Aplicar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="96e94-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="96e94-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96e94-157">None.</span></span>   |   <span data-ttu-id="96e94-158">Aplique as decisões de um accessReview concluído.</span><span class="sxs-lookup"><span data-stu-id="96e94-158">Apply the decisions from a completed accessReview.</span></span>|


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
