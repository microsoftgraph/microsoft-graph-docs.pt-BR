---
title: Listar meus decisões accessReview
description: No recurso de avaliações de acesso do Azure AD, recupere as decisões de um objeto accessReview para o usuário chamado como revisor.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525322"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="56af5-103">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="56af5-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56af5-104">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário chamado como revisor.</span><span class="sxs-lookup"><span data-stu-id="56af5-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="56af5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56af5-105">Permissions</span></span>
<span data-ttu-id="56af5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56af5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56af5-108">Permission type</span></span>                        | <span data-ttu-id="56af5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56af5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="56af5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56af5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56af5-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="56af5-111"></span></span>  <span data-ttu-id="56af5-112">O usuário conectado também deve ter permissão para ler este examinar acesso específico.</span><span class="sxs-lookup"><span data-stu-id="56af5-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="56af5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56af5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56af5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56af5-114">Not supported.</span></span> |
|<span data-ttu-id="56af5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56af5-115">Application</span></span>                            | <span data-ttu-id="56af5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56af5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56af5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56af5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="56af5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56af5-118">Request headers</span></span>
| <span data-ttu-id="56af5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="56af5-119">Name</span></span>         | <span data-ttu-id="56af5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="56af5-120">Type</span></span>        | <span data-ttu-id="56af5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="56af5-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="56af5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56af5-122">Authorization</span></span> | <span data-ttu-id="56af5-123">string</span><span class="sxs-lookup"><span data-stu-id="56af5-123">string</span></span> | <span data-ttu-id="56af5-124">Token de portador</span><span class="sxs-lookup"><span data-stu-id="56af5-124">Bearer \{token\}.</span></span> <span data-ttu-id="56af5-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56af5-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56af5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56af5-126">Request body</span></span>
<span data-ttu-id="56af5-127">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="56af5-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="56af5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="56af5-128">Response</span></span>
<span data-ttu-id="56af5-129">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário da chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="56af5-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="56af5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56af5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56af5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56af5-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="56af5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="56af5-132">Response</span></span>
><span data-ttu-id="56af5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56af5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="56af5-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="56af5-135">See also</span></span>

| <span data-ttu-id="56af5-136">Método</span><span class="sxs-lookup"><span data-stu-id="56af5-136">Method</span></span>           | <span data-ttu-id="56af5-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56af5-137">Return Type</span></span>    |<span data-ttu-id="56af5-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="56af5-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56af5-139">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="56af5-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="56af5-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="56af5-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="56af5-141">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="56af5-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="56af5-142">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="56af5-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="56af5-143">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="56af5-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="56af5-144">Recupere todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="56af5-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
