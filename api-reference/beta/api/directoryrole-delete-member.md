---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e194ee131c60be9d9563fac04e0ca1fb8f3b5c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957749"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="1fbc9-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="1fbc9-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fbc9-104">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fbc9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fbc9-105">Permissions</span></span>

<span data-ttu-id="1fbc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fbc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fbc9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fbc9-108">Permission type</span></span>      | <span data-ttu-id="1fbc9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fbc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fbc9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fbc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1fbc9-111">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="1fbc9-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fbc9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fbc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fbc9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-113">Not supported.</span></span>    |
|<span data-ttu-id="1fbc9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fbc9-114">Application</span></span> | <span data-ttu-id="1fbc9-115">RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="1fbc9-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fbc9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fbc9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1fbc9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbc9-117">Request headers</span></span>

| <span data-ttu-id="1fbc9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1fbc9-118">Name</span></span>       | <span data-ttu-id="1fbc9-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fbc9-119">Type</span></span> | <span data-ttu-id="1fbc9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fbc9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fbc9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fbc9-121">Authorization</span></span>  | <span data-ttu-id="1fbc9-122">string</span><span class="sxs-lookup"><span data-stu-id="1fbc9-122">string</span></span>  | <span data-ttu-id="1fbc9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fbc9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbc9-125">Request body</span></span>

<span data-ttu-id="1fbc9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fbc9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fbc9-127">Response</span></span>

<span data-ttu-id="1fbc9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fbc9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fbc9-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1fbc9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fbc9-131">Request</span></span>

<span data-ttu-id="1fbc9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1fbc9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fbc9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1fbc9-134">C#</span><span class="sxs-lookup"><span data-stu-id="1fbc9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fbc9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1fbc9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1fbc9-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1fbc9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1fbc9-137">Java</span><span class="sxs-lookup"><span data-stu-id="1fbc9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1fbc9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fbc9-138">Response</span></span>

<span data-ttu-id="1fbc9-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fbc9-139">Here is an example of the response.</span></span> 
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
