---
title: Delete extensionproperty
description: Excluir uma extensãoproperty.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 861a14fcd1aa7d9d61f6e14f30297d1138dbf40d
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289939"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="63bca-103">Delete extensionproperty</span><span class="sxs-lookup"><span data-stu-id="63bca-103">Delete extensionProperty</span></span>

<span data-ttu-id="63bca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63bca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63bca-105">Excluir uma [extensãoproperty](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="63bca-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="63bca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63bca-106">Permissions</span></span>

<span data-ttu-id="63bca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63bca-109">Permission type</span></span>      | <span data-ttu-id="63bca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63bca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63bca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63bca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63bca-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="63bca-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63bca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63bca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bca-114">Not supported.</span></span>    |
|<span data-ttu-id="63bca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63bca-115">Application</span></span> | <span data-ttu-id="63bca-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63bca-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63bca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63bca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63bca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63bca-118">Request headers</span></span>

| <span data-ttu-id="63bca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63bca-119">Name</span></span>       | <span data-ttu-id="63bca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63bca-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="63bca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="63bca-121">Authorization</span></span>  | <span data-ttu-id="63bca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63bca-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63bca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63bca-124">Request body</span></span>

<span data-ttu-id="63bca-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63bca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63bca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bca-126">Response</span></span>

<span data-ttu-id="63bca-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63bca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63bca-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="63bca-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63bca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63bca-130">Request</span></span>

<span data-ttu-id="63bca-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63bca-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63bca-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="63bca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="63bca-133">C#</span><span class="sxs-lookup"><span data-stu-id="63bca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63bca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63bca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63bca-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63bca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63bca-136">Java</span><span class="sxs-lookup"><span data-stu-id="63bca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63bca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bca-137">Response</span></span>

<span data-ttu-id="63bca-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63bca-138">The following is an example of the response.</span></span>

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
