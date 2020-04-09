---
title: Excluir oAuth2PermissionGrant
description: Excluir um oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 14d70a5673ddf1e08f9aa50758befb85348efa1a
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199981"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="bf890-103">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bf890-103">Delete oAuth2PermissionGrant</span></span>

<span data-ttu-id="bf890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf890-105">Excluir um oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="bf890-105">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf890-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf890-106">Permissions</span></span>
<span data-ttu-id="bf890-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf890-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf890-109">Permission type</span></span>      | <span data-ttu-id="bf890-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf890-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf890-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf890-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf890-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf890-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf890-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf890-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf890-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf890-114">Not supported.</span></span>    |
|<span data-ttu-id="bf890-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf890-115">Application</span></span> | <span data-ttu-id="bf890-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf890-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf890-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf890-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bf890-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf890-118">Request headers</span></span>
| <span data-ttu-id="bf890-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bf890-119">Name</span></span>       | <span data-ttu-id="bf890-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf890-120">Type</span></span> | <span data-ttu-id="bf890-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf890-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf890-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf890-122">Authorization</span></span>  | <span data-ttu-id="bf890-123">string</span><span class="sxs-lookup"><span data-stu-id="bf890-123">string</span></span>  | <span data-ttu-id="bf890-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf890-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf890-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf890-126">Request body</span></span>
<span data-ttu-id="bf890-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf890-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf890-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf890-128">Response</span></span>

<span data-ttu-id="bf890-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf890-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf890-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf890-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf890-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf890-132">Request</span></span>
<span data-ttu-id="bf890-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf890-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf890-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf890-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="bf890-135">C#</span><span class="sxs-lookup"><span data-stu-id="bf890-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf890-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf890-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf890-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf890-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf890-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf890-138">Response</span></span>
<span data-ttu-id="bf890-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf890-139">Here is an example of the response.</span></span> 
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
