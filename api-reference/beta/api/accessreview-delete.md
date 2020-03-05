---
title: Excluir accessReview
description: No recurso de revisões do Azure AD Access, exclua um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: daf96b917c8c285f06f803179c4c1eff5b913f86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441927"
---
# <a name="delete-accessreview"></a><span data-ttu-id="1a4e7-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="1a4e7-103">Delete accessReview</span></span>

<span data-ttu-id="1a4e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a4e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a4e7-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="1a4e7-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a4e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a4e7-106">Permissions</span></span>
<span data-ttu-id="1a4e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a4e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a4e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a4e7-109">Permission type</span></span>                        | <span data-ttu-id="1a4e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a4e7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a4e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a4e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a4e7-112">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1a4e7-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1a4e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a4e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a4e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a4e7-114">Not supported.</span></span> |
|<span data-ttu-id="1a4e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a4e7-115">Application</span></span>                            | <span data-ttu-id="1a4e7-116">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="1a4e7-116">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="1a4e7-117">O chamador também deve ter a permissão ProgramControl. ReadWrite. All, para que possa excluir um [ProgramControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="1a4e7-117">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="1a4e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a4e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="1a4e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4e7-119">Request headers</span></span>
| <span data-ttu-id="1a4e7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1a4e7-120">Name</span></span>         | <span data-ttu-id="1a4e7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a4e7-121">Type</span></span>        | <span data-ttu-id="1a4e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a4e7-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1a4e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a4e7-123">Authorization</span></span> | <span data-ttu-id="1a4e7-124">string</span><span class="sxs-lookup"><span data-stu-id="1a4e7-124">string</span></span> | <span data-ttu-id="1a4e7-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a4e7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a4e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4e7-127">Request body</span></span>
<span data-ttu-id="1a4e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a4e7-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1a4e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4e7-129">Response</span></span>
<span data-ttu-id="1a4e7-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a4e7-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a4e7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a4e7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a4e7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a4e7-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1a4e7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a4e7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="c"></a>[<span data-ttu-id="1a4e7-135">C#</span><span class="sxs-lookup"><span data-stu-id="1a4e7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a4e7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a4e7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a4e7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a4e7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a4e7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a4e7-138">Response</span></span>
><span data-ttu-id="1a4e7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a4e7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
