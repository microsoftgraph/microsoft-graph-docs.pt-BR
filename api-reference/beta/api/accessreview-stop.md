---
title: Parar accessReview
description: No recurso de revisões do Azure AD Access, interrompa um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.  Para impedir que uma revisão de acesso recorrente inicie instâncias futuras, atualize-a para alterar sua data de término agendada.  Depois que a revisão do Access for interrompida, os revisores não poderão mais fornecer entradas e as decisões de revisão do Access poderão ser aplicadas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40f659154c932dee35923d0622160c1ba0269399
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441837"
---
# <a name="stop-accessreview"></a><span data-ttu-id="1107a-106">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="1107a-106">Stop accessReview</span></span>

<span data-ttu-id="1107a-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1107a-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1107a-108">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , interrompa um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="1107a-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="1107a-109">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="1107a-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="1107a-110">Para impedir que uma revisão de acesso recorrente inicie instâncias futuras, [atualize-](accessreview-update.md) a para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="1107a-110">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="1107a-111">Depois que a revisão do Access for interrompida, os revisores não poderão mais fornecer entradas e as decisões de revisão do Access poderão ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="1107a-111">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="1107a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="1107a-112">Permissions</span></span>
<span data-ttu-id="1107a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1107a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1107a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1107a-115">Permission type</span></span>                        | <span data-ttu-id="1107a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1107a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1107a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1107a-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1107a-118">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1107a-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1107a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1107a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1107a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1107a-120">Not supported.</span></span> |
|<span data-ttu-id="1107a-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1107a-121">Application</span></span>                            | <span data-ttu-id="1107a-122">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="1107a-122">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1107a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1107a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="1107a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1107a-124">Request headers</span></span>
| <span data-ttu-id="1107a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1107a-125">Name</span></span>         | <span data-ttu-id="1107a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1107a-126">Type</span></span>        | <span data-ttu-id="1107a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1107a-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1107a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1107a-128">Authorization</span></span> | <span data-ttu-id="1107a-129">string</span><span class="sxs-lookup"><span data-stu-id="1107a-129">string</span></span> | <span data-ttu-id="1107a-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1107a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1107a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1107a-132">Request body</span></span>
<span data-ttu-id="1107a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1107a-133">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1107a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1107a-134">Response</span></span>
<span data-ttu-id="1107a-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1107a-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1107a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1107a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1107a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1107a-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1107a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1107a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="c"></a>[<span data-ttu-id="1107a-140">C#</span><span class="sxs-lookup"><span data-stu-id="1107a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1107a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1107a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1107a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1107a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1107a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1107a-143">Response</span></span>
><span data-ttu-id="1107a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1107a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
