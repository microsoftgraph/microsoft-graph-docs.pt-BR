---
title: SendReminder accessReview
description: 'No recurso de revisões do Azure AD Access, envie um lembrete para os revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 119d76fe4fe26ef48eb79ad736dfb99428574e24
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172695"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="9fd4a-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="9fd4a-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd4a-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , envie um lembrete para os revisores de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="9fd4a-106">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9fd4a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fd4a-107">Permissions</span></span>
<span data-ttu-id="9fd4a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fd4a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fd4a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fd4a-110">Permission type</span></span>                        | <span data-ttu-id="9fd4a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fd4a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fd4a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fd4a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fd4a-113">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fd4a-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9fd4a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fd4a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fd4a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-115">Not supported.</span></span> |
|<span data-ttu-id="9fd4a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fd4a-116">Application</span></span>                            | <span data-ttu-id="9fd4a-117">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="9fd4a-117">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fd4a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd4a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="9fd4a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd4a-119">Request headers</span></span>
| <span data-ttu-id="9fd4a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9fd4a-120">Name</span></span>         | <span data-ttu-id="9fd4a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd4a-121">Type</span></span>        | <span data-ttu-id="9fd4a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd4a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9fd4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fd4a-123">Authorization</span></span> | <span data-ttu-id="9fd4a-124">string</span><span class="sxs-lookup"><span data-stu-id="9fd4a-124">string</span></span> | <span data-ttu-id="9fd4a-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fd4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd4a-127">Request body</span></span>
<span data-ttu-id="9fd4a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9fd4a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd4a-129">Response</span></span>
<span data-ttu-id="9fd4a-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fd4a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fd4a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fd4a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd4a-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fd4a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd4a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fd4a-135">C#</span><span class="sxs-lookup"><span data-stu-id="9fd4a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fd4a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="9fd4a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fd4a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9fd4a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fd4a-138">Java</span><span class="sxs-lookup"><span data-stu-id="9fd4a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9fd4a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd4a-139">Response</span></span>
><span data-ttu-id="9fd4a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fd4a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
