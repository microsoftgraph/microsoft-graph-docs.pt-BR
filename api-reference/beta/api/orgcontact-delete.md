---
title: Excluir orgContact
description: Exclua orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30978ac456fb270bd114968dccfdadb808d4eace
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979882"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="5b497-103">Excluir orgContact</span><span class="sxs-lookup"><span data-stu-id="5b497-103">Delete orgContact</span></span>

<span data-ttu-id="5b497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b497-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b497-105">Exclua orgContact.</span><span class="sxs-lookup"><span data-stu-id="5b497-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b497-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b497-106">Permissions</span></span>
<span data-ttu-id="5b497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b497-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b497-109">Permission type</span></span>      | <span data-ttu-id="5b497-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b497-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b497-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b497-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b497-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b497-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b497-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b497-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b497-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b497-114">Not supported.</span></span>    |
|<span data-ttu-id="5b497-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b497-115">Application</span></span> | <span data-ttu-id="5b497-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b497-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b497-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b497-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5b497-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b497-118">Request headers</span></span>
| <span data-ttu-id="5b497-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5b497-119">Name</span></span>       | <span data-ttu-id="5b497-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b497-120">Type</span></span> | <span data-ttu-id="5b497-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b497-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b497-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b497-122">Authorization</span></span>  | <span data-ttu-id="5b497-123">string</span><span class="sxs-lookup"><span data-stu-id="5b497-123">string</span></span>  | <span data-ttu-id="5b497-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b497-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b497-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b497-126">Request body</span></span>
<span data-ttu-id="5b497-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b497-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b497-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b497-128">Response</span></span>

<span data-ttu-id="5b497-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b497-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b497-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b497-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b497-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b497-132">Request</span></span>
<span data-ttu-id="5b497-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b497-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b497-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b497-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="5b497-135">C#</span><span class="sxs-lookup"><span data-stu-id="5b497-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b497-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b497-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b497-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b497-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5b497-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b497-138">Response</span></span>
<span data-ttu-id="5b497-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b497-139">Here is an example of the response.</span></span> 
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


