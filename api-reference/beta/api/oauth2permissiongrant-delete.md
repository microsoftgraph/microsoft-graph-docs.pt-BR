---
title: Excluir oAuth2PermissionGrant
description: Excluir um oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 92deefab9f561e35ba09ff302a8c881592c32381
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878974"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="1e150-103">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1e150-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e150-104">Excluir um oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="1e150-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e150-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e150-105">Permissions</span></span>
<span data-ttu-id="1e150-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e150-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e150-108">Permission type</span></span>      | <span data-ttu-id="1e150-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e150-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e150-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e150-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e150-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e150-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e150-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e150-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e150-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e150-113">Not supported.</span></span>    |
|<span data-ttu-id="1e150-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e150-114">Application</span></span> | <span data-ttu-id="1e150-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e150-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e150-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e150-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1e150-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e150-117">Request headers</span></span>
| <span data-ttu-id="1e150-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1e150-118">Name</span></span>       | <span data-ttu-id="1e150-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e150-119">Type</span></span> | <span data-ttu-id="1e150-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e150-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e150-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e150-121">Authorization</span></span>  | <span data-ttu-id="1e150-122">string</span><span class="sxs-lookup"><span data-stu-id="1e150-122">string</span></span>  | <span data-ttu-id="1e150-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e150-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e150-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e150-125">Request body</span></span>
<span data-ttu-id="1e150-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e150-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e150-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e150-127">Response</span></span>

<span data-ttu-id="1e150-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e150-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e150-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e150-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e150-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e150-131">Request</span></span>
<span data-ttu-id="1e150-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e150-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e150-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e150-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e150-134">C#</span><span class="sxs-lookup"><span data-stu-id="1e150-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e150-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e150-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e150-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1e150-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e150-137">Java</span><span class="sxs-lookup"><span data-stu-id="1e150-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1e150-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e150-138">Response</span></span>
<span data-ttu-id="1e150-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e150-139">Here is an example of the response.</span></span> 
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
