---
title: Excluir registeredUsers
description: Remover um usuário como um usuário registrado do dispositivo.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45a185f71b93fa7ad5a5d791839487c7ab9b14e4
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "45224791"
---
# <a name="delete-registereduser"></a><span data-ttu-id="0cb57-103">Excluir registeredUser</span><span class="sxs-lookup"><span data-stu-id="0cb57-103">Delete registeredUser</span></span>

<span data-ttu-id="0cb57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb57-105">Remover um usuário como um usuário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0cb57-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cb57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cb57-106">Permissions</span></span>

<span data-ttu-id="0cb57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cb57-109">Permission type</span></span>      | <span data-ttu-id="0cb57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cb57-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cb57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cb57-111">Delegated (work or school account)</span></span> |<span data-ttu-id="0cb57-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cb57-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cb57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cb57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cb57-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cb57-114">Not supported.</span></span>    |
|<span data-ttu-id="0cb57-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cb57-115">Application</span></span> | <span data-ttu-id="0cb57-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb57-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0cb57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb57-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0cb57-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb57-118">Request headers</span></span>
| <span data-ttu-id="0cb57-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0cb57-119">Name</span></span>       | <span data-ttu-id="0cb57-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cb57-120">Type</span></span> | <span data-ttu-id="0cb57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cb57-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0cb57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cb57-122">Authorization</span></span>  | <span data-ttu-id="0cb57-123">string</span><span class="sxs-lookup"><span data-stu-id="0cb57-123">string</span></span>  | <span data-ttu-id="0cb57-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cb57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cb57-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb57-126">Request body</span></span>
<span data-ttu-id="0cb57-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cb57-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cb57-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb57-128">Response</span></span>

<span data-ttu-id="0cb57-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0cb57-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0cb57-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cb57-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cb57-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb57-131">Request</span></span>
<span data-ttu-id="0cb57-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cb57-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cb57-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb57-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0cb57-134">C#</span><span class="sxs-lookup"><span data-stu-id="0cb57-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cb57-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cb57-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cb57-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cb57-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="0cb57-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb57-137">Response</span></span>
<span data-ttu-id="0cb57-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cb57-138">Here is an example of the response.</span></span>
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
