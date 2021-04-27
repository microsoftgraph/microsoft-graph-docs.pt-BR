---
title: Parar accessReview
description: No recurso de análises de acesso do Azure AD, pare um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  (Para impedir que uma revisão de acesso recorrente inseja instâncias futuras, atualize-a para alterar sua data de término agendada).  Depois que a revisão de acesso parar, os revisadores não poderão mais dar entrada e as decisões de revisão de acesso podem ser aplicadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 44a6449012f3ac1032f8c442280b8aff58cb009b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048446"
---
# <a name="stop-accessreview"></a><span data-ttu-id="595ef-106">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="595ef-106">Stop accessReview</span></span>

<span data-ttu-id="595ef-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="595ef-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="595ef-108">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) pare um [accessReview ativo no momento.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="595ef-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="595ef-109">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="595ef-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="595ef-110">(Para impedir que uma revisão de acesso recorrente inseja instâncias futuras, [atualize-a](accessreview-update.md) para alterar sua data de término agendada).</span><span class="sxs-lookup"><span data-stu-id="595ef-110">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="595ef-111">Depois que a revisão de acesso parar, os revisadores não poderão mais dar entrada e as decisões de revisão de acesso podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="595ef-111">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="595ef-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="595ef-112">Permissions</span></span>
<span data-ttu-id="595ef-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="595ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="595ef-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="595ef-115">Permission type</span></span>                        | <span data-ttu-id="595ef-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="595ef-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="595ef-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="595ef-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="595ef-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="595ef-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="595ef-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="595ef-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="595ef-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="595ef-120">Not supported.</span></span> |
|<span data-ttu-id="595ef-121">Application</span><span class="sxs-lookup"><span data-stu-id="595ef-121">Application</span></span>                            | <span data-ttu-id="595ef-122">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="595ef-122">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="595ef-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="595ef-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="595ef-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="595ef-124">Request headers</span></span>
| <span data-ttu-id="595ef-125">Nome</span><span class="sxs-lookup"><span data-stu-id="595ef-125">Name</span></span>         | <span data-ttu-id="595ef-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="595ef-126">Type</span></span>        | <span data-ttu-id="595ef-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="595ef-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="595ef-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="595ef-128">Authorization</span></span> | <span data-ttu-id="595ef-129">string</span><span class="sxs-lookup"><span data-stu-id="595ef-129">string</span></span> | <span data-ttu-id="595ef-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="595ef-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="595ef-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="595ef-132">Request body</span></span>
<span data-ttu-id="595ef-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="595ef-133">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="595ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="595ef-134">Response</span></span>
<span data-ttu-id="595ef-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="595ef-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="595ef-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="595ef-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="595ef-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="595ef-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="595ef-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="595ef-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="c"></a>[<span data-ttu-id="595ef-140">C#</span><span class="sxs-lookup"><span data-stu-id="595ef-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="595ef-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="595ef-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="595ef-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="595ef-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="595ef-143">Java</span><span class="sxs-lookup"><span data-stu-id="595ef-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="595ef-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="595ef-144">Response</span></span>
><span data-ttu-id="595ef-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="595ef-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


