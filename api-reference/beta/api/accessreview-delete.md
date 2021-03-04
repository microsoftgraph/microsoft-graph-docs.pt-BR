---
title: Excluir accessReview
description: No recurso de análises de acesso do Azure AD, exclua um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e5ece558893b20ec4d514c24e540799a1ea4762f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439412"
---
# <a name="delete-accessreview"></a><span data-ttu-id="67fed-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="67fed-103">Delete accessReview</span></span>

<span data-ttu-id="67fed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67fed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67fed-105">No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) exclua um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="67fed-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67fed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67fed-106">Permissions</span></span>
<span data-ttu-id="67fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67fed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67fed-109">Permission type</span></span>                        | <span data-ttu-id="67fed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67fed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="67fed-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67fed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="67fed-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fed-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="67fed-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67fed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67fed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67fed-114">Not supported.</span></span> |
|<span data-ttu-id="67fed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67fed-115">Application</span></span>                            | <span data-ttu-id="67fed-116">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="67fed-116">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="67fed-117">O chamador também deve ter permissão ProgramControl.ReadWrite.All, para que ele possa excluir um [programControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="67fed-117">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="67fed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67fed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="67fed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67fed-119">Request headers</span></span>
| <span data-ttu-id="67fed-120">Nome</span><span class="sxs-lookup"><span data-stu-id="67fed-120">Name</span></span>         | <span data-ttu-id="67fed-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="67fed-121">Type</span></span>        | <span data-ttu-id="67fed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="67fed-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="67fed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67fed-123">Authorization</span></span> | <span data-ttu-id="67fed-124">string</span><span class="sxs-lookup"><span data-stu-id="67fed-124">string</span></span> | <span data-ttu-id="67fed-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67fed-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67fed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67fed-127">Request body</span></span>
<span data-ttu-id="67fed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67fed-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="67fed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="67fed-129">Response</span></span>
<span data-ttu-id="67fed-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67fed-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67fed-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67fed-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67fed-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67fed-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="67fed-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="67fed-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="c"></a>[<span data-ttu-id="67fed-135">C#</span><span class="sxs-lookup"><span data-stu-id="67fed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67fed-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67fed-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67fed-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67fed-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67fed-138">Java</span><span class="sxs-lookup"><span data-stu-id="67fed-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67fed-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="67fed-139">Response</span></span>
><span data-ttu-id="67fed-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67fed-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


