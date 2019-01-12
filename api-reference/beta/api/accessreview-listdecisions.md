---
title: Lista accessReview decisões
description: No Windows Azure AD para acessar o recurso de revisões, recuperar as decisões de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927006"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="74586-103">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="74586-103">List accessReview decisions</span></span>

> <span data-ttu-id="74586-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="74586-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74586-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="74586-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74586-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="74586-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="74586-107">Observe que uma análise mais acesso recorrente não terá um `decisions` relacionamento.</span><span class="sxs-lookup"><span data-stu-id="74586-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="74586-108">Em vez disso, o chamador deve navegar o `instance` relação para encontrar um `accessReview` objeto para uma instância atual ou passado da revisão acesso.</span><span class="sxs-lookup"><span data-stu-id="74586-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="74586-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="74586-109">Permissions</span></span>
<span data-ttu-id="74586-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74586-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74586-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74586-112">Permission type</span></span>                        | <span data-ttu-id="74586-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74586-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74586-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74586-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="74586-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="74586-115"></span></span>  <span data-ttu-id="74586-116">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="74586-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="74586-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74586-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74586-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74586-118">Not supported.</span></span> |
|<span data-ttu-id="74586-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74586-119">Application</span></span>                            | <span data-ttu-id="74586-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74586-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74586-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74586-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="74586-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74586-122">Request headers</span></span>
| <span data-ttu-id="74586-123">Nome</span><span class="sxs-lookup"><span data-stu-id="74586-123">Name</span></span>         | <span data-ttu-id="74586-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="74586-124">Type</span></span>        | <span data-ttu-id="74586-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="74586-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="74586-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="74586-126">Authorization</span></span> | <span data-ttu-id="74586-127">string</span><span class="sxs-lookup"><span data-stu-id="74586-127">string</span></span> | <span data-ttu-id="74586-128">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="74586-128">Bearer \{token\}.</span></span> <span data-ttu-id="74586-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74586-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74586-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74586-130">Request body</span></span>
<span data-ttu-id="74586-131">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="74586-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="74586-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="74586-132">Response</span></span>
<span data-ttu-id="74586-133">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74586-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74586-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74586-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74586-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74586-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="74586-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="74586-136">Response</span></span>
><span data-ttu-id="74586-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74586-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="74586-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="74586-139">See also</span></span>

| <span data-ttu-id="74586-140">Método</span><span class="sxs-lookup"><span data-stu-id="74586-140">Method</span></span>           | <span data-ttu-id="74586-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74586-141">Return Type</span></span>    |<span data-ttu-id="74586-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="74586-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74586-143">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="74586-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="74586-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="74586-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="74586-145">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="74586-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="74586-146">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="74586-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="74586-147">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="74586-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="74586-148">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="74586-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="74586-149">Enviar accessReview lembrete</span><span class="sxs-lookup"><span data-stu-id="74586-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="74586-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74586-150">None.</span></span>   |   <span data-ttu-id="74586-151">Envie um lembrete para os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="74586-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="74586-152">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="74586-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="74586-153">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74586-153">None.</span></span>   |   <span data-ttu-id="74586-154">Pare uma accessReview.</span><span class="sxs-lookup"><span data-stu-id="74586-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="74586-155">Redefinir accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="74586-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="74586-156">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74586-156">None.</span></span>   |   <span data-ttu-id="74586-157">Redefina as decisões em um accessReview em andamento.</span><span class="sxs-lookup"><span data-stu-id="74586-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="74586-158">Aplicar accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="74586-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="74586-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74586-159">None.</span></span>   |   <span data-ttu-id="74586-160">Aplique as decisões de um accessReview concluída.</span><span class="sxs-lookup"><span data-stu-id="74586-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
