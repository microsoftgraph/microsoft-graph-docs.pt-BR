---
title: Excluir extensionProperty
description: Exclua uma extensionProperty.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08a4cbd6478edb4a24d9e26318c8becef3e0f92c
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844631"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="484dc-103">Excluir extensionProperty</span><span class="sxs-lookup"><span data-stu-id="484dc-103">Delete extensionProperty</span></span>

<span data-ttu-id="484dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="484dc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="484dc-105">[Exclua uma extensionProperty](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="484dc-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="484dc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="484dc-106">Permissions</span></span>

<span data-ttu-id="484dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="484dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="484dc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="484dc-109">Permission type</span></span>      | <span data-ttu-id="484dc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="484dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="484dc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="484dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="484dc-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="484dc-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="484dc-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="484dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="484dc-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="484dc-114">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="484dc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="484dc-115">Application</span></span> | <span data-ttu-id="484dc-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="484dc-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="484dc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="484dc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="484dc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-118">Request headers</span></span>

| <span data-ttu-id="484dc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="484dc-119">Name</span></span>       | <span data-ttu-id="484dc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="484dc-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="484dc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="484dc-121">Authorization</span></span>  | <span data-ttu-id="484dc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="484dc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="484dc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-124">Request body</span></span>

<span data-ttu-id="484dc-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="484dc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="484dc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="484dc-126">Response</span></span>

<span data-ttu-id="484dc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="484dc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="484dc-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="484dc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="484dc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="484dc-130">Request</span></span>

<span data-ttu-id="484dc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="484dc-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="484dc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="484dc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="484dc-133">C#</span><span class="sxs-lookup"><span data-stu-id="484dc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="484dc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="484dc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="484dc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="484dc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="484dc-136">Java</span><span class="sxs-lookup"><span data-stu-id="484dc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="484dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="484dc-137">Response</span></span>

<span data-ttu-id="484dc-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="484dc-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

