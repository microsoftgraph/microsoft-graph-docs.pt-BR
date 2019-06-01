---
title: Excluir directoryObject
description: Exclui um directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d550a12839bdb1bb6520edd35ef08e0322d8e2fe
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657011"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="15843-103">Excluir directoryObject</span><span class="sxs-lookup"><span data-stu-id="15843-103">Delete directoryObject</span></span>

<span data-ttu-id="15843-104">Exclui um directoryObject.</span><span class="sxs-lookup"><span data-stu-id="15843-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="15843-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="15843-105">Permissions</span></span>
<span data-ttu-id="15843-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15843-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="15843-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15843-108">Permission type</span></span>      | <span data-ttu-id="15843-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15843-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15843-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15843-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15843-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15843-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15843-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15843-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15843-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15843-113">Not supported.</span></span>    |
|<span data-ttu-id="15843-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15843-114">Application</span></span> | <span data-ttu-id="15843-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15843-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15843-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15843-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="15843-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15843-117">Request headers</span></span>
| <span data-ttu-id="15843-118">Nome</span><span class="sxs-lookup"><span data-stu-id="15843-118">Name</span></span>       | <span data-ttu-id="15843-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="15843-119">Type</span></span> | <span data-ttu-id="15843-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="15843-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15843-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15843-121">Authorization</span></span>  | <span data-ttu-id="15843-122">string</span><span class="sxs-lookup"><span data-stu-id="15843-122">string</span></span>  | <span data-ttu-id="15843-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15843-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15843-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15843-125">Request body</span></span>
<span data-ttu-id="15843-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15843-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15843-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="15843-127">Response</span></span>

<span data-ttu-id="15843-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15843-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15843-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15843-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15843-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15843-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="15843-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="15843-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="15843-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15843-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15843-134">C#</span><span class="sxs-lookup"><span data-stu-id="15843-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15843-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="15843-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
