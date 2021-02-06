---
title: Excluir extensionProperty
description: Exclua uma extensionProperty.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ce1b58d22d58a261f1725bd304be01e5e27478ae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129286"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="efd70-103">Excluir extensionProperty</span><span class="sxs-lookup"><span data-stu-id="efd70-103">Delete extensionProperty</span></span>

<span data-ttu-id="efd70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd70-105">[Exclua uma extensionProperty](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="efd70-105">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="efd70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="efd70-106">Permissions</span></span>

<span data-ttu-id="efd70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efd70-109">Permission type</span></span>      | <span data-ttu-id="efd70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efd70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd70-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efd70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efd70-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="efd70-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="efd70-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efd70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd70-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd70-114">Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="efd70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efd70-115">Application</span></span> | <span data-ttu-id="efd70-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd70-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efd70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efd70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="efd70-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efd70-118">Request headers</span></span>

| <span data-ttu-id="efd70-119">Nome</span><span class="sxs-lookup"><span data-stu-id="efd70-119">Name</span></span>       | <span data-ttu-id="efd70-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd70-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="efd70-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="efd70-121">Authorization</span></span>  | <span data-ttu-id="efd70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efd70-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efd70-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efd70-124">Request body</span></span>

<span data-ttu-id="efd70-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efd70-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd70-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd70-126">Response</span></span>

<span data-ttu-id="efd70-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efd70-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efd70-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="efd70-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efd70-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efd70-130">Request</span></span>

<span data-ttu-id="efd70-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="efd70-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="efd70-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd70-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="efd70-133">C#</span><span class="sxs-lookup"><span data-stu-id="efd70-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efd70-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd70-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efd70-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd70-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efd70-136">Java</span><span class="sxs-lookup"><span data-stu-id="efd70-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="efd70-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd70-137">Response</span></span>

<span data-ttu-id="efd70-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="efd70-138">The following is an example of the response.</span></span>

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



