---
title: Excluir uma configuração de grupo
description: Excluir uma configuração de grupo.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f3b65b7f41e5a53ebada692347fdc53fbf986267
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679782"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="54caf-103">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="54caf-103">Delete a group setting</span></span>

<span data-ttu-id="54caf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54caf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54caf-105">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="54caf-105">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="54caf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54caf-106">Permissions</span></span>

<span data-ttu-id="54caf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54caf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54caf-109">Permission type</span></span>      | <span data-ttu-id="54caf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54caf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54caf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54caf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54caf-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54caf-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54caf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54caf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54caf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54caf-114">Not supported.</span></span>    |
|<span data-ttu-id="54caf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54caf-115">Application</span></span> | <span data-ttu-id="54caf-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54caf-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54caf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54caf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="54caf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54caf-118">Request headers</span></span>

| <span data-ttu-id="54caf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54caf-119">Name</span></span> | <span data-ttu-id="54caf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54caf-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="54caf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54caf-121">Authorization</span></span>  | <span data-ttu-id="54caf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54caf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54caf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54caf-124">Content-Type</span></span>  | <span data-ttu-id="54caf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54caf-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="54caf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54caf-126">Request body</span></span>
<span data-ttu-id="54caf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54caf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54caf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="54caf-128">Response</span></span>

<span data-ttu-id="54caf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54caf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54caf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54caf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54caf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54caf-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="54caf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="54caf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="54caf-134">C#</span><span class="sxs-lookup"><span data-stu-id="54caf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54caf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54caf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54caf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54caf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54caf-137">Java</span><span class="sxs-lookup"><span data-stu-id="54caf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54caf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="54caf-138">Response</span></span>
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

