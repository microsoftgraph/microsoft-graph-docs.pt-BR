---
title: Excluir orgContact
description: Exclua orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f28a2e61325caa2c44189697efc06224ca386576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467020"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="94fab-103">Excluir orgContact</span><span class="sxs-lookup"><span data-stu-id="94fab-103">Delete orgContact</span></span>

<span data-ttu-id="94fab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94fab-105">Exclua orgContact.</span><span class="sxs-lookup"><span data-stu-id="94fab-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="94fab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94fab-106">Permissions</span></span>
<span data-ttu-id="94fab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94fab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94fab-109">Permission type</span></span>      | <span data-ttu-id="94fab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94fab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94fab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94fab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94fab-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94fab-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94fab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94fab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94fab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94fab-114">Not supported.</span></span>    |
|<span data-ttu-id="94fab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94fab-115">Application</span></span> | <span data-ttu-id="94fab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94fab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94fab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94fab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="94fab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94fab-118">Request headers</span></span>
| <span data-ttu-id="94fab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="94fab-119">Name</span></span>       | <span data-ttu-id="94fab-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="94fab-120">Type</span></span> | <span data-ttu-id="94fab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94fab-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94fab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94fab-122">Authorization</span></span>  | <span data-ttu-id="94fab-123">string</span><span class="sxs-lookup"><span data-stu-id="94fab-123">string</span></span>  | <span data-ttu-id="94fab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94fab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94fab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94fab-126">Request body</span></span>
<span data-ttu-id="94fab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94fab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94fab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fab-128">Response</span></span>

<span data-ttu-id="94fab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94fab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94fab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94fab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fab-132">Request</span></span>
<span data-ttu-id="94fab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94fab-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94fab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94fab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="94fab-135">C#</span><span class="sxs-lookup"><span data-stu-id="94fab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94fab-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94fab-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94fab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94fab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94fab-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fab-138">Response</span></span>
<span data-ttu-id="94fab-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fab-139">Here is an example of the response.</span></span> 
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
