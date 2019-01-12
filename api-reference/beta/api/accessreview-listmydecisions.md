---
title: Listar meus decisões accessReview
description: No recurso de avaliações de acesso do Azure AD, recupere as decisões de um objeto accessReview para o usuário chamado como revisor.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 037b916bca45c74d1918b45e4e9e21b685bd8ae0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941496"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="58f7d-103">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="58f7d-103">List my accessReview decisions</span></span>

> <span data-ttu-id="58f7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58f7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58f7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58f7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58f7d-106">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário chamado como revisor.</span><span class="sxs-lookup"><span data-stu-id="58f7d-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="58f7d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="58f7d-107">Permissions</span></span>
<span data-ttu-id="58f7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f7d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58f7d-110">Permission type</span></span>                        | <span data-ttu-id="58f7d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58f7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="58f7d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58f7d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="58f7d-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="58f7d-113"></span></span>  <span data-ttu-id="58f7d-114">O usuário conectado também deve ter permissão para ler este examinar acesso específico.</span><span class="sxs-lookup"><span data-stu-id="58f7d-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="58f7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58f7d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58f7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58f7d-116">Not supported.</span></span> |
|<span data-ttu-id="58f7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58f7d-117">Application</span></span>                            | <span data-ttu-id="58f7d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58f7d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58f7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58f7d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="58f7d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58f7d-120">Request headers</span></span>
| <span data-ttu-id="58f7d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="58f7d-121">Name</span></span>         | <span data-ttu-id="58f7d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="58f7d-122">Type</span></span>        | <span data-ttu-id="58f7d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f7d-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="58f7d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58f7d-124">Authorization</span></span> | <span data-ttu-id="58f7d-125">string</span><span class="sxs-lookup"><span data-stu-id="58f7d-125">string</span></span> | <span data-ttu-id="58f7d-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="58f7d-126">Bearer \{token\}.</span></span> <span data-ttu-id="58f7d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58f7d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58f7d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58f7d-128">Request body</span></span>
<span data-ttu-id="58f7d-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="58f7d-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="58f7d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f7d-130">Response</span></span>
<span data-ttu-id="58f7d-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário da chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="58f7d-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="58f7d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58f7d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58f7d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58f7d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="58f7d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="58f7d-134">Response</span></span>
><span data-ttu-id="58f7d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58f7d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="58f7d-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="58f7d-137">See also</span></span>

| <span data-ttu-id="58f7d-138">Método</span><span class="sxs-lookup"><span data-stu-id="58f7d-138">Method</span></span>           | <span data-ttu-id="58f7d-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="58f7d-139">Return Type</span></span>    |<span data-ttu-id="58f7d-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="58f7d-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58f7d-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="58f7d-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="58f7d-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="58f7d-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="58f7d-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="58f7d-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="58f7d-144">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="58f7d-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="58f7d-145">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="58f7d-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="58f7d-146">Recupere todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="58f7d-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
