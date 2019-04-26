---
title: Listar minhas decisões do accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview para o usuário de chamada como revisor.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a493f746cd7b69b77fe038d992d4b6e7d387e296
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323648"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="d004f-103">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="d004f-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d004f-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário de chamada como revisor.</span><span class="sxs-lookup"><span data-stu-id="d004f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="d004f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d004f-105">Permissions</span></span>
<span data-ttu-id="d004f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d004f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d004f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d004f-108">Permission type</span></span>                        | <span data-ttu-id="d004f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d004f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d004f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d004f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d004f-111">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d004f-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="d004f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d004f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d004f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d004f-113">Not supported.</span></span> |
|<span data-ttu-id="d004f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d004f-114">Application</span></span>                            | <span data-ttu-id="d004f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d004f-115">Not supported.</span></span> |

<span data-ttu-id="d004f-116">O usuário conectado também deve ter permissão para ler essa revisão de acesso específica.</span><span class="sxs-lookup"><span data-stu-id="d004f-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d004f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d004f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="d004f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d004f-118">Request headers</span></span>
| <span data-ttu-id="d004f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d004f-119">Name</span></span>         | <span data-ttu-id="d004f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d004f-120">Type</span></span>        | <span data-ttu-id="d004f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d004f-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d004f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d004f-122">Authorization</span></span> | <span data-ttu-id="d004f-123">string</span><span class="sxs-lookup"><span data-stu-id="d004f-123">string</span></span> | <span data-ttu-id="d004f-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d004f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d004f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d004f-126">Request body</span></span>
<span data-ttu-id="d004f-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="d004f-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d004f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d004f-128">Response</span></span>
<span data-ttu-id="d004f-129">Se bem-sucedido, este método retorna um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="d004f-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="d004f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d004f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d004f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d004f-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="d004f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d004f-132">Response</span></span>
><span data-ttu-id="d004f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d004f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d004f-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="d004f-135">See also</span></span>

| <span data-ttu-id="d004f-136">Método</span><span class="sxs-lookup"><span data-stu-id="d004f-136">Method</span></span>           | <span data-ttu-id="d004f-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d004f-137">Return Type</span></span>    |<span data-ttu-id="d004f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d004f-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d004f-139">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="d004f-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d004f-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="d004f-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d004f-141">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="d004f-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d004f-142">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="d004f-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d004f-143">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="d004f-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d004f-144">Recuperar todas as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="d004f-144">Retrieve all the decisions of an accessReview.</span></span>|


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
