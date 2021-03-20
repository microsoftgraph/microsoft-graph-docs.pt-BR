---
title: SendReminder accessReview
description: 'No recurso de revisões de acesso do Azure AD, envie um lembrete aos revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bab89d572bac3df90065693bcb8886f1271b7480
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943098"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="50e2c-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="50e2c-104">SendReminder accessReview</span></span>

<span data-ttu-id="50e2c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50e2c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50e2c-106">No recurso de revisões de acesso do Azure AD, envie um lembrete aos [revisores](../resources/accessreviews-root.md) de um [accessReview ativo no momento.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="50e2c-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="50e2c-107">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="50e2c-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="50e2c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="50e2c-108">Permissions</span></span>
<span data-ttu-id="50e2c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50e2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50e2c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50e2c-111">Permission type</span></span>                        | <span data-ttu-id="50e2c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50e2c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="50e2c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50e2c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="50e2c-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50e2c-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="50e2c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50e2c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50e2c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50e2c-116">Not supported.</span></span> |
|<span data-ttu-id="50e2c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50e2c-117">Application</span></span>                            | <span data-ttu-id="50e2c-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="50e2c-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="50e2c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50e2c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="50e2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50e2c-120">Request headers</span></span>
| <span data-ttu-id="50e2c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="50e2c-121">Name</span></span>         | <span data-ttu-id="50e2c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="50e2c-122">Type</span></span>        | <span data-ttu-id="50e2c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="50e2c-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="50e2c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="50e2c-124">Authorization</span></span> | <span data-ttu-id="50e2c-125">string</span><span class="sxs-lookup"><span data-stu-id="50e2c-125">string</span></span> | <span data-ttu-id="50e2c-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50e2c-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50e2c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50e2c-128">Request body</span></span>
<span data-ttu-id="50e2c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50e2c-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="50e2c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="50e2c-130">Response</span></span>
<span data-ttu-id="50e2c-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50e2c-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50e2c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50e2c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50e2c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50e2c-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="50e2c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="50e2c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_1"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="50e2c-136">C#</span><span class="sxs-lookup"><span data-stu-id="50e2c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50e2c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50e2c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50e2c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50e2c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50e2c-139">Java</span><span class="sxs-lookup"><span data-stu-id="50e2c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50e2c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="50e2c-140">Response</span></span>
><span data-ttu-id="50e2c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50e2c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


