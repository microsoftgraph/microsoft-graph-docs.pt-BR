---
title: Excluir orgContact
description: Exclua orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 612a56c7fdf35ddb8e6b6eefc6b89c3830c700aa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414324"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="15cc0-103">Excluir orgContact</span><span class="sxs-lookup"><span data-stu-id="15cc0-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15cc0-104">Exclua orgContact.</span><span class="sxs-lookup"><span data-stu-id="15cc0-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="15cc0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="15cc0-105">Permissions</span></span>
<span data-ttu-id="15cc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15cc0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15cc0-108">Permission type</span></span>      | <span data-ttu-id="15cc0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15cc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15cc0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15cc0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="15cc0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15cc0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15cc0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15cc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15cc0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15cc0-113">Not supported.</span></span>    |
|<span data-ttu-id="15cc0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cc0-114">Application</span></span> | <span data-ttu-id="15cc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15cc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15cc0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15cc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="15cc0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15cc0-117">Request headers</span></span>
| <span data-ttu-id="15cc0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="15cc0-118">Name</span></span>       | <span data-ttu-id="15cc0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="15cc0-119">Type</span></span> | <span data-ttu-id="15cc0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="15cc0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15cc0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15cc0-121">Authorization</span></span>  | <span data-ttu-id="15cc0-122">string</span><span class="sxs-lookup"><span data-stu-id="15cc0-122">string</span></span>  | <span data-ttu-id="15cc0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15cc0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15cc0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15cc0-125">Request body</span></span>
<span data-ttu-id="15cc0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15cc0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15cc0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="15cc0-127">Response</span></span>

<span data-ttu-id="15cc0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15cc0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15cc0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15cc0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15cc0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15cc0-131">Request</span></span>
<span data-ttu-id="15cc0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15cc0-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15cc0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="15cc0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15cc0-134">C#</span><span class="sxs-lookup"><span data-stu-id="15cc0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15cc0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15cc0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15cc0-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15cc0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15cc0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="15cc0-137">Response</span></span>
<span data-ttu-id="15cc0-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15cc0-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
