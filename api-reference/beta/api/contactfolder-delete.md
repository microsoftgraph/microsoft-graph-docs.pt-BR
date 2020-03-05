---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 313716931f282661c93c297ec72dcbbba915fdfc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437004"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="59f80-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="59f80-103">Delete contactFolder</span></span>

<span data-ttu-id="59f80-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59f80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59f80-105">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="59f80-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="59f80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59f80-106">Permissions</span></span>
<span data-ttu-id="59f80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59f80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59f80-109">Permission type</span></span>      | <span data-ttu-id="59f80-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59f80-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59f80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59f80-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59f80-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59f80-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59f80-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59f80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59f80-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59f80-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59f80-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59f80-115">Application</span></span> | <span data-ttu-id="59f80-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59f80-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59f80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f80-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59f80-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59f80-118">Request headers</span></span>
| <span data-ttu-id="59f80-119">Nome</span><span class="sxs-lookup"><span data-stu-id="59f80-119">Name</span></span>       | <span data-ttu-id="59f80-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f80-120">Type</span></span> | <span data-ttu-id="59f80-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f80-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59f80-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59f80-122">Authorization</span></span>  | <span data-ttu-id="59f80-123">string</span><span class="sxs-lookup"><span data-stu-id="59f80-123">string</span></span>  | <span data-ttu-id="59f80-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59f80-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59f80-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f80-126">Request body</span></span>
<span data-ttu-id="59f80-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59f80-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59f80-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f80-128">Response</span></span>

<span data-ttu-id="59f80-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f80-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f80-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f80-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59f80-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59f80-132">Request</span></span>
<span data-ttu-id="59f80-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59f80-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59f80-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59f80-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="59f80-135">C#</span><span class="sxs-lookup"><span data-stu-id="59f80-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59f80-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59f80-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59f80-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59f80-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59f80-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f80-138">Response</span></span>
<span data-ttu-id="59f80-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f80-139">Here is an example of the response.</span></span> 
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
