---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 18c3a64c1ec00b2ad385ac6c33e94d7d4df699d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057606"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="839e6-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="839e6-103">Delete contactFolder</span></span>

<span data-ttu-id="839e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="839e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="839e6-105">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="839e6-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="839e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="839e6-106">Permissions</span></span>
<span data-ttu-id="839e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="839e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="839e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="839e6-109">Permission type</span></span>      | <span data-ttu-id="839e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="839e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="839e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="839e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="839e6-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839e6-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="839e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="839e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="839e6-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839e6-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="839e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="839e6-115">Application</span></span> | <span data-ttu-id="839e6-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839e6-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="839e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="839e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="839e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="839e6-118">Request headers</span></span>
| <span data-ttu-id="839e6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="839e6-119">Name</span></span>       | <span data-ttu-id="839e6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="839e6-120">Type</span></span> | <span data-ttu-id="839e6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="839e6-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="839e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="839e6-122">Authorization</span></span>  | <span data-ttu-id="839e6-123">string</span><span class="sxs-lookup"><span data-stu-id="839e6-123">string</span></span>  | <span data-ttu-id="839e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="839e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="839e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="839e6-126">Request body</span></span>
<span data-ttu-id="839e6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="839e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="839e6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="839e6-128">Response</span></span>

<span data-ttu-id="839e6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="839e6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="839e6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="839e6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="839e6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="839e6-132">Request</span></span>
<span data-ttu-id="839e6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="839e6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="839e6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="839e6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="839e6-135">C#</span><span class="sxs-lookup"><span data-stu-id="839e6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="839e6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="839e6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="839e6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="839e6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="839e6-138">Java</span><span class="sxs-lookup"><span data-stu-id="839e6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="839e6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="839e6-139">Response</span></span>
<span data-ttu-id="839e6-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="839e6-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

