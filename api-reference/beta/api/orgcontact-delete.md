---
title: Excluir orgContact
description: Exclua orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b95d9db3e86851f3e510775a5fba7a15fc1435a1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346512"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="add35-103">Excluir orgContact</span><span class="sxs-lookup"><span data-stu-id="add35-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="add35-104">Exclua orgContact.</span><span class="sxs-lookup"><span data-stu-id="add35-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="add35-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="add35-105">Permissions</span></span>
<span data-ttu-id="add35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="add35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="add35-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="add35-108">Permission type</span></span>      | <span data-ttu-id="add35-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="add35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="add35-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="add35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="add35-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="add35-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="add35-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="add35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="add35-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add35-113">Not supported.</span></span>    |
|<span data-ttu-id="add35-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="add35-114">Application</span></span> | <span data-ttu-id="add35-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="add35-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="add35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="add35-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="add35-117">Request headers</span></span>
| <span data-ttu-id="add35-118">Nome</span><span class="sxs-lookup"><span data-stu-id="add35-118">Name</span></span>       | <span data-ttu-id="add35-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="add35-119">Type</span></span> | <span data-ttu-id="add35-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="add35-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="add35-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="add35-121">Authorization</span></span>  | <span data-ttu-id="add35-122">string</span><span class="sxs-lookup"><span data-stu-id="add35-122">string</span></span>  | <span data-ttu-id="add35-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="add35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="add35-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="add35-125">Request body</span></span>
<span data-ttu-id="add35-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="add35-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="add35-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="add35-127">Response</span></span>

<span data-ttu-id="add35-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="add35-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="add35-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="add35-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="add35-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="add35-131">Request</span></span>
<span data-ttu-id="add35-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="add35-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="add35-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="add35-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="add35-134">C#</span><span class="sxs-lookup"><span data-stu-id="add35-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="add35-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add35-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="add35-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="add35-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="add35-137">Java</span><span class="sxs-lookup"><span data-stu-id="add35-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="add35-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="add35-138">Response</span></span>
<span data-ttu-id="add35-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="add35-139">Here is an example of the response.</span></span> 
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
