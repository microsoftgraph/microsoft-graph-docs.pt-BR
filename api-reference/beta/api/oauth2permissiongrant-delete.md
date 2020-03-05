---
title: Excluir oAuth2PermissionGrant
description: Excluir um oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3bc0786445e8bac495a0768751ac43fb1ead5bb4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456688"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="7f383-103">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="7f383-103">Delete oAuth2PermissionGrant</span></span>

<span data-ttu-id="7f383-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f383-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f383-105">Excluir um oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="7f383-105">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f383-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f383-106">Permissions</span></span>
<span data-ttu-id="7f383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f383-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f383-109">Permission type</span></span>      | <span data-ttu-id="7f383-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f383-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f383-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f383-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f383-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f383-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f383-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f383-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f383-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f383-114">Not supported.</span></span>    |
|<span data-ttu-id="7f383-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f383-115">Application</span></span> | <span data-ttu-id="7f383-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f383-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f383-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f383-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7f383-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f383-118">Request headers</span></span>
| <span data-ttu-id="7f383-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7f383-119">Name</span></span>       | <span data-ttu-id="7f383-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f383-120">Type</span></span> | <span data-ttu-id="7f383-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f383-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f383-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f383-122">Authorization</span></span>  | <span data-ttu-id="7f383-123">string</span><span class="sxs-lookup"><span data-stu-id="7f383-123">string</span></span>  | <span data-ttu-id="7f383-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f383-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f383-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f383-126">Request body</span></span>
<span data-ttu-id="7f383-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f383-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f383-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f383-128">Response</span></span>

<span data-ttu-id="7f383-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f383-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f383-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f383-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f383-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f383-132">Request</span></span>
<span data-ttu-id="7f383-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f383-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f383-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f383-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="7f383-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f383-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f383-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f383-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f383-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f383-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f383-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f383-138">Response</span></span>
<span data-ttu-id="7f383-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f383-139">Here is an example of the response.</span></span> 
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
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
