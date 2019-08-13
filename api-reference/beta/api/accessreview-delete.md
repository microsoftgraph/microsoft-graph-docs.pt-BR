---
title: Excluir accessReview
description: No recurso de revisões do Azure AD Access, exclua um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ded5c3776dbc66a6433482a40fb95ec248c2f95
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316116"
---
# <a name="delete-accessreview"></a><span data-ttu-id="a07c1-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="a07c1-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a07c1-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a07c1-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a07c1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a07c1-105">Permissions</span></span>
<span data-ttu-id="a07c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07c1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a07c1-108">Permission type</span></span>                        | <span data-ttu-id="a07c1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a07c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a07c1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a07c1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a07c1-111">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a07c1-111">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a07c1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a07c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a07c1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a07c1-113">Not supported.</span></span> |
|<span data-ttu-id="a07c1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a07c1-114">Application</span></span>                            | <span data-ttu-id="a07c1-115">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="a07c1-115">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="a07c1-116">O chamador também deve ter a permissão ProgramControl. ReadWrite. All, para que possa excluir um [ProgramControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="a07c1-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="a07c1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a07c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="a07c1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a07c1-118">Request headers</span></span>
| <span data-ttu-id="a07c1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a07c1-119">Name</span></span>         | <span data-ttu-id="a07c1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a07c1-120">Type</span></span>        | <span data-ttu-id="a07c1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a07c1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a07c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a07c1-122">Authorization</span></span> | <span data-ttu-id="a07c1-123">string</span><span class="sxs-lookup"><span data-stu-id="a07c1-123">string</span></span> | <span data-ttu-id="a07c1-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a07c1-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a07c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a07c1-126">Request body</span></span>
<span data-ttu-id="a07c1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a07c1-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a07c1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a07c1-128">Response</span></span>
<span data-ttu-id="a07c1-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a07c1-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07c1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a07c1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a07c1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a07c1-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a07c1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a07c1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a07c1-134">C#</span><span class="sxs-lookup"><span data-stu-id="a07c1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a07c1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a07c1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a07c1-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a07c1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a07c1-137">Java</span><span class="sxs-lookup"><span data-stu-id="a07c1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a07c1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a07c1-138">Response</span></span>
><span data-ttu-id="a07c1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a07c1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
