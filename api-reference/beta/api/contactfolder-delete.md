---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 587941fd8463971c593caa045b17759b10758d00
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996322"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="5c306-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="5c306-103">Delete contactFolder</span></span>

<span data-ttu-id="5c306-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c306-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c306-105">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="5c306-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c306-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c306-106">Permissions</span></span>
<span data-ttu-id="5c306-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c306-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c306-109">Permission type</span></span>      | <span data-ttu-id="5c306-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c306-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c306-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c306-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c306-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c306-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5c306-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c306-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c306-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c306-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="5c306-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c306-115">Application</span></span> | <span data-ttu-id="5c306-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c306-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c306-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c306-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5c306-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c306-118">Request headers</span></span>
| <span data-ttu-id="5c306-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c306-119">Name</span></span>       | <span data-ttu-id="5c306-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c306-120">Type</span></span> | <span data-ttu-id="5c306-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c306-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c306-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c306-122">Authorization</span></span>  | <span data-ttu-id="5c306-123">string</span><span class="sxs-lookup"><span data-stu-id="5c306-123">string</span></span>  | <span data-ttu-id="5c306-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c306-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c306-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c306-126">Request body</span></span>
<span data-ttu-id="5c306-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c306-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c306-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c306-128">Response</span></span>

<span data-ttu-id="5c306-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c306-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c306-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c306-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c306-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c306-132">Request</span></span>
<span data-ttu-id="5c306-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c306-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c306-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c306-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="5c306-135">C#</span><span class="sxs-lookup"><span data-stu-id="5c306-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c306-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c306-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c306-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c306-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c306-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c306-138">Response</span></span>
<span data-ttu-id="5c306-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c306-139">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


