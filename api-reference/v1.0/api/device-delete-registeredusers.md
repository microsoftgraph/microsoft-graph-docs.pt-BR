---
title: Excluir registeredUsers
description: Remova um usuário como um usuário registrado do dispositivo.
localization_priority: Normal
author: michaelrm97
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 78f5755e249a6a83f040cb6ad31aaccde8b010f6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434647"
---
# <a name="delete-registereduser"></a><span data-ttu-id="d6ce3-103">Excluir registeredUser</span><span class="sxs-lookup"><span data-stu-id="d6ce3-103">Delete registeredUser</span></span>

<span data-ttu-id="d6ce3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ce3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6ce3-105">Remova um usuário como um usuário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6ce3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6ce3-106">Permissions</span></span>

<span data-ttu-id="d6ce3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6ce3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6ce3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6ce3-109">Permission type</span></span>      | <span data-ttu-id="d6ce3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6ce3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6ce3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6ce3-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d6ce3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6ce3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6ce3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6ce3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ce3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-114">Not supported.</span></span>    |
|<span data-ttu-id="d6ce3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6ce3-115">Application</span></span> | <span data-ttu-id="d6ce3-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ce3-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d6ce3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ce3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d6ce3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce3-118">Request headers</span></span>
| <span data-ttu-id="d6ce3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d6ce3-119">Name</span></span>       | <span data-ttu-id="d6ce3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ce3-120">Type</span></span> | <span data-ttu-id="d6ce3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ce3-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6ce3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6ce3-122">Authorization</span></span>  | <span data-ttu-id="d6ce3-123">string</span><span class="sxs-lookup"><span data-stu-id="d6ce3-123">string</span></span>  | <span data-ttu-id="d6ce3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6ce3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce3-126">Request body</span></span>
<span data-ttu-id="d6ce3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6ce3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ce3-128">Response</span></span>

<span data-ttu-id="d6ce3-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6ce3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6ce3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6ce3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ce3-131">Request</span></span>
<span data-ttu-id="d6ce3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6ce3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ce3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="d6ce3-134">C#</span><span class="sxs-lookup"><span data-stu-id="d6ce3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6ce3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6ce3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6ce3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6ce3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6ce3-137">Java</span><span class="sxs-lookup"><span data-stu-id="d6ce3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="d6ce3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ce3-138">Response</span></span>
<span data-ttu-id="d6ce3-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6ce3-139">Here is an example of the response.</span></span>
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
  "description": "Delete registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

