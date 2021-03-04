---
title: Excluir orgContact
description: Excluir orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b853a153afea17bae86a7e0d4215f9ae0ac39db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434018"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="54887-103">Excluir orgContact</span><span class="sxs-lookup"><span data-stu-id="54887-103">Delete orgContact</span></span>

<span data-ttu-id="54887-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54887-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54887-105">Excluir orgContact.</span><span class="sxs-lookup"><span data-stu-id="54887-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="54887-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54887-106">Permissions</span></span>
<span data-ttu-id="54887-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54887-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54887-109">Permission type</span></span>      | <span data-ttu-id="54887-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54887-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54887-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54887-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54887-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54887-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54887-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54887-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54887-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54887-114">Not supported.</span></span>    |
|<span data-ttu-id="54887-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54887-115">Application</span></span> | <span data-ttu-id="54887-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54887-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54887-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54887-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="54887-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54887-118">Request headers</span></span>
| <span data-ttu-id="54887-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54887-119">Name</span></span>       | <span data-ttu-id="54887-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="54887-120">Type</span></span> | <span data-ttu-id="54887-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="54887-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="54887-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54887-122">Authorization</span></span>  | <span data-ttu-id="54887-123">string</span><span class="sxs-lookup"><span data-stu-id="54887-123">string</span></span>  | <span data-ttu-id="54887-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54887-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54887-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54887-126">Request body</span></span>
<span data-ttu-id="54887-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54887-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54887-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="54887-128">Response</span></span>

<span data-ttu-id="54887-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54887-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54887-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54887-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54887-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54887-132">Request</span></span>
<span data-ttu-id="54887-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54887-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54887-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="54887-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="54887-135">C#</span><span class="sxs-lookup"><span data-stu-id="54887-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54887-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54887-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54887-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54887-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54887-138">Java</span><span class="sxs-lookup"><span data-stu-id="54887-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54887-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="54887-139">Response</span></span>
<span data-ttu-id="54887-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54887-140">Here is an example of the response.</span></span> 
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


