---
title: Listar meus decisões accessReview
description: No recurso de avaliações de acesso do Azure AD, recupere as decisões de um objeto accessReview para o usuário chamado como revisor.
localization_priority: Normal
ms.openlocfilehash: 27ae3129810b6019ecf47e23f1e4cc48362df6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819008"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="d198e-103">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="d198e-103">List my accessReview decisions</span></span>

> <span data-ttu-id="d198e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d198e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d198e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d198e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d198e-106">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário chamado como revisor.</span><span class="sxs-lookup"><span data-stu-id="d198e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="d198e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d198e-107">Permissions</span></span>
<span data-ttu-id="d198e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d198e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d198e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d198e-110">Permission type</span></span>                        | <span data-ttu-id="d198e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d198e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d198e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d198e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d198e-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d198e-113"></span></span>  <span data-ttu-id="d198e-114">O usuário conectado também deve ter permissão para ler este examinar acesso específico.</span><span class="sxs-lookup"><span data-stu-id="d198e-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="d198e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d198e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d198e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d198e-116">Not supported.</span></span> |
|<span data-ttu-id="d198e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d198e-117">Application</span></span>                            | <span data-ttu-id="d198e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d198e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d198e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d198e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="d198e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d198e-120">Request headers</span></span>
| <span data-ttu-id="d198e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d198e-121">Name</span></span>         | <span data-ttu-id="d198e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d198e-122">Type</span></span>        | <span data-ttu-id="d198e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d198e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d198e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d198e-124">Authorization</span></span> | <span data-ttu-id="d198e-125">string</span><span class="sxs-lookup"><span data-stu-id="d198e-125">string</span></span> | <span data-ttu-id="d198e-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="d198e-126">Bearer \{token\}.</span></span> <span data-ttu-id="d198e-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d198e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d198e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d198e-128">Request body</span></span>
<span data-ttu-id="d198e-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d198e-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d198e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d198e-130">Response</span></span>
<span data-ttu-id="d198e-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário da chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="d198e-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="d198e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d198e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d198e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d198e-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="d198e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d198e-134">Response</span></span>
><span data-ttu-id="d198e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d198e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d198e-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d198e-137">See also</span></span>

| <span data-ttu-id="d198e-138">Método</span><span class="sxs-lookup"><span data-stu-id="d198e-138">Method</span></span>           | <span data-ttu-id="d198e-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d198e-139">Return Type</span></span>    |<span data-ttu-id="d198e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="d198e-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d198e-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="d198e-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d198e-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="d198e-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d198e-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d198e-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d198e-144">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="d198e-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d198e-145">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="d198e-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d198e-146">Recupere todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d198e-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
