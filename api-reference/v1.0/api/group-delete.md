---
title: Excluir grupo - API Graph Microsoft
description: Excluir um recurso de grupo.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a81560df24820aaa79a9fb7d4adebcc7e4d89ecb
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680952"
---
# <a name="delete-group"></a><span data-ttu-id="40c7d-103">Excluir grupo</span><span class="sxs-lookup"><span data-stu-id="40c7d-103">Delete group</span></span>

<span data-ttu-id="40c7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40c7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40c7d-105">Exclua o grupo.</span><span class="sxs-lookup"><span data-stu-id="40c7d-105">Delete group.</span></span>  

<span data-ttu-id="40c7d-106">Quando excluídos, Microsoft 365 grupos são movidos para um contêiner temporário e podem ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="40c7d-106">When deleted, Microsoft 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="40c7d-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="40c7d-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="40c7d-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="40c7d-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="40c7d-109">Isso se aplica somente Microsoft 365 grupos.</span><span class="sxs-lookup"><span data-stu-id="40c7d-109">This applies only to Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="40c7d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="40c7d-110">Permissions</span></span>

<span data-ttu-id="40c7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40c7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40c7d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40c7d-113">Permission type</span></span>      | <span data-ttu-id="40c7d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40c7d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40c7d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40c7d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="40c7d-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40c7d-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="40c7d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40c7d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40c7d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40c7d-118">Not supported.</span></span>    |
|<span data-ttu-id="40c7d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40c7d-119">Application</span></span> | <span data-ttu-id="40c7d-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40c7d-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40c7d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40c7d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40c7d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40c7d-122">Request headers</span></span>

| <span data-ttu-id="40c7d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="40c7d-123">Name</span></span>       | <span data-ttu-id="40c7d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="40c7d-124">Type</span></span> | <span data-ttu-id="40c7d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="40c7d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40c7d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="40c7d-126">Authorization</span></span>  | <span data-ttu-id="40c7d-127">string</span><span class="sxs-lookup"><span data-stu-id="40c7d-127">string</span></span>  | <span data-ttu-id="40c7d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40c7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40c7d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40c7d-130">Request body</span></span>

<span data-ttu-id="40c7d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40c7d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40c7d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="40c7d-132">Response</span></span>

<span data-ttu-id="40c7d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40c7d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40c7d-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40c7d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="40c7d-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40c7d-136">Request</span></span>

<span data-ttu-id="40c7d-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40c7d-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40c7d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="40c7d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="c"></a>[<span data-ttu-id="40c7d-139">C#</span><span class="sxs-lookup"><span data-stu-id="40c7d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40c7d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40c7d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40c7d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40c7d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40c7d-142">Java</span><span class="sxs-lookup"><span data-stu-id="40c7d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40c7d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="40c7d-143">Response</span></span>

<span data-ttu-id="40c7d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40c7d-144">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

