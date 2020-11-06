---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3af5d5079971b0e15fe0ecaab971c28d297de03
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932343"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="f6156-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="f6156-103">Remove directory role member</span></span>

<span data-ttu-id="f6156-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6156-105">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="f6156-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6156-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6156-106">Permissions</span></span>

<span data-ttu-id="f6156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6156-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6156-109">Permission type</span></span>      | <span data-ttu-id="f6156-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6156-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6156-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6156-112">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f6156-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6156-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6156-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6156-114">Not supported.</span></span>    |
|<span data-ttu-id="f6156-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6156-115">Application</span></span> | <span data-ttu-id="f6156-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f6156-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6156-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6156-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f6156-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6156-118">Request headers</span></span>

| <span data-ttu-id="f6156-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f6156-119">Name</span></span>       | <span data-ttu-id="f6156-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6156-120">Type</span></span> | <span data-ttu-id="f6156-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6156-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6156-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6156-122">Authorization</span></span>  | <span data-ttu-id="f6156-123">string</span><span class="sxs-lookup"><span data-stu-id="f6156-123">string</span></span>  | <span data-ttu-id="f6156-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6156-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6156-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6156-126">Request body</span></span>

<span data-ttu-id="f6156-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6156-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6156-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6156-128">Response</span></span>

<span data-ttu-id="f6156-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6156-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6156-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6156-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6156-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6156-132">Request</span></span>

<span data-ttu-id="f6156-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6156-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6156-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6156-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f6156-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6156-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6156-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6156-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6156-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6156-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6156-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6156-138">Response</span></span>

<span data-ttu-id="f6156-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6156-139">Here is an example of the response.</span></span> 
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


