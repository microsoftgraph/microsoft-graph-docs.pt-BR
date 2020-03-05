---
title: SendReminder accessReview
description: 'No recurso de revisões do Azure AD Access, envie um lembrete para os revisores de um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 41d82fe28405c5068a10cd5780bd115b293e6e71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441848"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="75cbb-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="75cbb-104">SendReminder accessReview</span></span>

<span data-ttu-id="75cbb-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="75cbb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75cbb-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , envie um lembrete para os revisores de um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="75cbb-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="75cbb-107">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="75cbb-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="75cbb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="75cbb-108">Permissions</span></span>
<span data-ttu-id="75cbb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75cbb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75cbb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75cbb-111">Permission type</span></span>                        | <span data-ttu-id="75cbb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75cbb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="75cbb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75cbb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="75cbb-114">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="75cbb-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="75cbb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75cbb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75cbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75cbb-116">Not supported.</span></span> |
|<span data-ttu-id="75cbb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75cbb-117">Application</span></span>                            | <span data-ttu-id="75cbb-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="75cbb-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="75cbb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75cbb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="75cbb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75cbb-120">Request headers</span></span>
| <span data-ttu-id="75cbb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="75cbb-121">Name</span></span>         | <span data-ttu-id="75cbb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="75cbb-122">Type</span></span>        | <span data-ttu-id="75cbb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="75cbb-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="75cbb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="75cbb-124">Authorization</span></span> | <span data-ttu-id="75cbb-125">string</span><span class="sxs-lookup"><span data-stu-id="75cbb-125">string</span></span> | <span data-ttu-id="75cbb-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75cbb-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75cbb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75cbb-128">Request body</span></span>
<span data-ttu-id="75cbb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75cbb-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="75cbb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="75cbb-130">Response</span></span>
<span data-ttu-id="75cbb-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75cbb-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75cbb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75cbb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75cbb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75cbb-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="75cbb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="75cbb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="75cbb-136">C#</span><span class="sxs-lookup"><span data-stu-id="75cbb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75cbb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75cbb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75cbb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75cbb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75cbb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="75cbb-139">Response</span></span>
><span data-ttu-id="75cbb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75cbb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
