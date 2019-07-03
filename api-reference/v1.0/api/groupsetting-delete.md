---
title: Excluir uma configuração de grupo
description: Excluir uma configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8b7ad2acdff3148a4cbbd6f6415d7ef8aa9161f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447408"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="092c0-103">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="092c0-103">Delete a group setting</span></span>

<span data-ttu-id="092c0-104">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="092c0-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="092c0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="092c0-105">Permissions</span></span>

<span data-ttu-id="092c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="092c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="092c0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="092c0-108">Permission type</span></span>      | <span data-ttu-id="092c0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="092c0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="092c0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="092c0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="092c0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="092c0-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="092c0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="092c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="092c0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="092c0-113">Not supported.</span></span>    |
|<span data-ttu-id="092c0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="092c0-114">Application</span></span> | <span data-ttu-id="092c0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="092c0-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="092c0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="092c0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="092c0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="092c0-117">Request headers</span></span>

| <span data-ttu-id="092c0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="092c0-118">Name</span></span> | <span data-ttu-id="092c0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="092c0-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="092c0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="092c0-120">Authorization</span></span>  | <span data-ttu-id="092c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="092c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="092c0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="092c0-123">Content-Type</span></span>  | <span data-ttu-id="092c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="092c0-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="092c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="092c0-125">Request body</span></span>
<span data-ttu-id="092c0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="092c0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="092c0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="092c0-127">Response</span></span>

<span data-ttu-id="092c0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="092c0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="092c0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="092c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="092c0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="092c0-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="092c0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="092c0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="092c0-133">C#</span><span class="sxs-lookup"><span data-stu-id="092c0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="092c0-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="092c0-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="092c0-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="092c0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="092c0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="092c0-136">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
