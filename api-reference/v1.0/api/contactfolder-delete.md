---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cf70727a5960a37982522f158bc1b0d4cfac46c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462172"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="c36be-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="c36be-103">Delete contactFolder</span></span>

<span data-ttu-id="c36be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c36be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c36be-105">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="c36be-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c36be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c36be-106">Permissions</span></span>
<span data-ttu-id="c36be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c36be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c36be-109">Permission type</span></span>      | <span data-ttu-id="c36be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c36be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c36be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c36be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c36be-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c36be-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c36be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c36be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c36be-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c36be-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c36be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c36be-115">Application</span></span> | <span data-ttu-id="c36be-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c36be-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c36be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c36be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c36be-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c36be-118">Request headers</span></span>
| <span data-ttu-id="c36be-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c36be-119">Name</span></span>       | <span data-ttu-id="c36be-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c36be-120">Type</span></span> | <span data-ttu-id="c36be-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c36be-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c36be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c36be-122">Authorization</span></span>  | <span data-ttu-id="c36be-123">string</span><span class="sxs-lookup"><span data-stu-id="c36be-123">string</span></span>  | <span data-ttu-id="c36be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c36be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c36be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c36be-126">Request body</span></span>
<span data-ttu-id="c36be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c36be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c36be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36be-128">Response</span></span>

<span data-ttu-id="c36be-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c36be-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c36be-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c36be-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c36be-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c36be-132">Request</span></span>
<span data-ttu-id="c36be-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c36be-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c36be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c36be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="c36be-135">C#</span><span class="sxs-lookup"><span data-stu-id="c36be-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c36be-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c36be-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c36be-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c36be-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c36be-138">Java</span><span class="sxs-lookup"><span data-stu-id="c36be-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c36be-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36be-139">Response</span></span>
<span data-ttu-id="c36be-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c36be-140">Here is an example of the response.</span></span> 
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
