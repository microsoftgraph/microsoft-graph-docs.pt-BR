---
title: Excluir accessReview
description: No recurso de revisões do Azure AD Access, exclua um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e401dc19b4ea541e5c286298a6b02c0d773dd80b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655478"
---
# <a name="delete-accessreview"></a><span data-ttu-id="5a2f0-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="5a2f0-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a2f0-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , exclua um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2f0-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a2f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a2f0-105">Permissions</span></span>
<span data-ttu-id="5a2f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a2f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a2f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a2f0-108">Permission type</span></span>                        | <span data-ttu-id="5a2f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a2f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a2f0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a2f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a2f0-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2f0-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="5a2f0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a2f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a2f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-113">Not supported.</span></span> |
|<span data-ttu-id="5a2f0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a2f0-114">Application</span></span>                            | <span data-ttu-id="5a2f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-115">Not supported.</span></span> |

<span data-ttu-id="5a2f0-116">O chamador também deve ter a permissão ProgramControl. ReadWrite. All, para que possa excluir um [ProgramControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="5a2f0-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="5a2f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a2f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="5a2f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2f0-118">Request headers</span></span>
| <span data-ttu-id="5a2f0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5a2f0-119">Name</span></span>         | <span data-ttu-id="5a2f0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a2f0-120">Type</span></span>        | <span data-ttu-id="5a2f0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2f0-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5a2f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a2f0-122">Authorization</span></span> | <span data-ttu-id="5a2f0-123">string</span><span class="sxs-lookup"><span data-stu-id="5a2f0-123">string</span></span> | <span data-ttu-id="5a2f0-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a2f0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2f0-126">Request body</span></span>
<span data-ttu-id="5a2f0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5a2f0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2f0-128">Response</span></span>
<span data-ttu-id="5a2f0-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2f0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a2f0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a2f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2f0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
##### <a name="response"></a><span data-ttu-id="5a2f0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2f0-133">Response</span></span>
><span data-ttu-id="5a2f0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a2f0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a2f0-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5a2f0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a2f0-137">C#</span><span class="sxs-lookup"><span data-stu-id="5a2f0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a2f0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a2f0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
