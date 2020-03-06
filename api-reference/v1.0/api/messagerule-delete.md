---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b4b30165fe69971f9b22d828708bf1e352d80397
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511457"
---
# <a name="delete-messagerule"></a><span data-ttu-id="6af62-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="6af62-103">Delete messageRule</span></span>

<span data-ttu-id="6af62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af62-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6af62-105">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="6af62-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6af62-106">Permissions</span></span>
<span data-ttu-id="6af62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6af62-109">Permission type</span></span>      | <span data-ttu-id="6af62-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6af62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6af62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6af62-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af62-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6af62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6af62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af62-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af62-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6af62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6af62-115">Application</span></span> | <span data-ttu-id="6af62-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6af62-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6af62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6af62-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6af62-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6af62-118">Request headers</span></span>
| <span data-ttu-id="6af62-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6af62-119">Name</span></span>       | <span data-ttu-id="6af62-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6af62-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6af62-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6af62-121">Authorization</span></span>  | <span data-ttu-id="6af62-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af62-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6af62-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6af62-124">Request body</span></span>
<span data-ttu-id="6af62-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6af62-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6af62-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af62-126">Response</span></span>
<span data-ttu-id="6af62-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af62-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6af62-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6af62-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6af62-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6af62-130">Request</span></span>
<span data-ttu-id="6af62-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6af62-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6af62-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6af62-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="c"></a>[<span data-ttu-id="6af62-133">C#</span><span class="sxs-lookup"><span data-stu-id="6af62-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6af62-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6af62-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6af62-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6af62-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6af62-136">Java</span><span class="sxs-lookup"><span data-stu-id="6af62-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6af62-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af62-137">Response</span></span>
<span data-ttu-id="6af62-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af62-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
