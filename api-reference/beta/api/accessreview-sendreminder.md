---
title: SendReminder accessReview
description: 'No recurso de revisões de acesso do Azure AD, envie um lembrete aos revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 18036576918a1a1259df8aa95386fcac34ce54b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048453"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="585d8-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="585d8-104">SendReminder accessReview</span></span>

<span data-ttu-id="585d8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="585d8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585d8-106">No recurso de revisões de acesso do Azure AD, envie um lembrete aos [revisores](../resources/accessreviews-root.md) de um [accessReview ativo no momento.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="585d8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="585d8-107">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="585d8-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="585d8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="585d8-108">Permissions</span></span>
<span data-ttu-id="585d8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="585d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="585d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="585d8-111">Permission type</span></span>                        | <span data-ttu-id="585d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="585d8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="585d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="585d8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="585d8-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="585d8-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="585d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="585d8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="585d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="585d8-116">Not supported.</span></span> |
|<span data-ttu-id="585d8-117">Application</span><span class="sxs-lookup"><span data-stu-id="585d8-117">Application</span></span>                            | <span data-ttu-id="585d8-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="585d8-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="585d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="585d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="585d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="585d8-120">Request headers</span></span>
| <span data-ttu-id="585d8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="585d8-121">Name</span></span>         | <span data-ttu-id="585d8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="585d8-122">Type</span></span>        | <span data-ttu-id="585d8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="585d8-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="585d8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="585d8-124">Authorization</span></span> | <span data-ttu-id="585d8-125">string</span><span class="sxs-lookup"><span data-stu-id="585d8-125">string</span></span> | <span data-ttu-id="585d8-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="585d8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="585d8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="585d8-128">Request body</span></span>
<span data-ttu-id="585d8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="585d8-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="585d8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="585d8-130">Response</span></span>
<span data-ttu-id="585d8-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="585d8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="585d8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="585d8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="585d8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="585d8-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="585d8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="585d8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_1"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="585d8-136">C#</span><span class="sxs-lookup"><span data-stu-id="585d8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="585d8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="585d8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="585d8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="585d8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="585d8-139">Java</span><span class="sxs-lookup"><span data-stu-id="585d8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="585d8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="585d8-140">Response</span></span>
><span data-ttu-id="585d8-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="585d8-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


