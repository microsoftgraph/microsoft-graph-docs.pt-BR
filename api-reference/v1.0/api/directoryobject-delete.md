---
title: Excluir directoryObject
description: Exclui um directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 79d76974479981a74d6b05d66febf413154d8dab
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275604"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="24be6-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="24be6-103">Delete directoryObject</span></span>

<span data-ttu-id="24be6-104">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="24be6-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="24be6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24be6-105">Permissions</span></span>
<span data-ttu-id="24be6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24be6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="24be6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24be6-108">Permission type</span></span>      | <span data-ttu-id="24be6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24be6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24be6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24be6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24be6-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24be6-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24be6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24be6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24be6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24be6-113">Not supported.</span></span>    |
|<span data-ttu-id="24be6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24be6-114">Application</span></span> | <span data-ttu-id="24be6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24be6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24be6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24be6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="24be6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24be6-117">Request headers</span></span>
| <span data-ttu-id="24be6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="24be6-118">Name</span></span>       | <span data-ttu-id="24be6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="24be6-119">Type</span></span> | <span data-ttu-id="24be6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24be6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24be6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24be6-121">Authorization</span></span>  | <span data-ttu-id="24be6-122">string</span><span class="sxs-lookup"><span data-stu-id="24be6-122">string</span></span>  | <span data-ttu-id="24be6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24be6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24be6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24be6-125">Request body</span></span>
<span data-ttu-id="24be6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24be6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24be6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24be6-127">Response</span></span>

<span data-ttu-id="24be6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24be6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24be6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24be6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24be6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24be6-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="24be6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24be6-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24be6-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24be6-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24be6-134">C#</span><span class="sxs-lookup"><span data-stu-id="24be6-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24be6-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="24be6-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="24be6-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="24be6-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
