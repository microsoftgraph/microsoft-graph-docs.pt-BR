---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fac71741248db5d92691aa8592ff6ac2178284d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008803"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="faeac-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="faeac-103">Remove directory role member</span></span>

<span data-ttu-id="faeac-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="faeac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faeac-105">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="faeac-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="faeac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="faeac-106">Permissions</span></span>

<span data-ttu-id="faeac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faeac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="faeac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faeac-109">Permission type</span></span>      | <span data-ttu-id="faeac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="faeac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faeac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faeac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="faeac-112">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="faeac-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="faeac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faeac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faeac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faeac-114">Not supported.</span></span>    |
|<span data-ttu-id="faeac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faeac-115">Application</span></span> | <span data-ttu-id="faeac-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="faeac-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="faeac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faeac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="faeac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faeac-118">Request headers</span></span>

| <span data-ttu-id="faeac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="faeac-119">Name</span></span>       | <span data-ttu-id="faeac-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="faeac-120">Type</span></span> | <span data-ttu-id="faeac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="faeac-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="faeac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="faeac-122">Authorization</span></span>  | <span data-ttu-id="faeac-123">string</span><span class="sxs-lookup"><span data-stu-id="faeac-123">string</span></span>  | <span data-ttu-id="faeac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faeac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faeac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faeac-126">Request body</span></span>

<span data-ttu-id="faeac-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="faeac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faeac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="faeac-128">Response</span></span>

<span data-ttu-id="faeac-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faeac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faeac-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faeac-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="faeac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faeac-132">Request</span></span>

<span data-ttu-id="faeac-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="faeac-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="faeac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="faeac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="faeac-135">C#</span><span class="sxs-lookup"><span data-stu-id="faeac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="faeac-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="faeac-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="faeac-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="faeac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="faeac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="faeac-138">Response</span></span>

<span data-ttu-id="faeac-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faeac-139">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


