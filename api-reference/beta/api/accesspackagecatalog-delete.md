---
title: Excluir accessPackageCatalog
description: Exclua accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0eb63d30abe92025d9a6ce23e123bf3bd3d5164d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441995"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="ff6f3-103">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="ff6f3-103">Delete accessPackageCatalog</span></span>

<span data-ttu-id="ff6f3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff6f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff6f3-105">Excluir um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="ff6f3-105">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff6f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff6f3-106">Permissions</span></span>

<span data-ttu-id="ff6f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff6f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff6f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff6f3-109">Permission type</span></span>                        | <span data-ttu-id="ff6f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff6f3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ff6f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff6f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff6f3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff6f3-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ff6f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff6f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff6f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-114">Not supported.</span></span> |
| <span data-ttu-id="ff6f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff6f3-115">Application</span></span>                            | <span data-ttu-id="ff6f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff6f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6f3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ff6f3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff6f3-118">Request headers</span></span>

| <span data-ttu-id="ff6f3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ff6f3-119">Name</span></span>          | <span data-ttu-id="ff6f3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff6f3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ff6f3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff6f3-121">Authorization</span></span> | <span data-ttu-id="ff6f3-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-122">Bearer \{token\}.</span></span> <span data-ttu-id="ff6f3-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff6f3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff6f3-124">Request body</span></span>

<span data-ttu-id="ff6f3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff6f3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff6f3-126">Response</span></span>

<span data-ttu-id="ff6f3-127">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-127">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="ff6f3-128">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff6f3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff6f3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff6f3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff6f3-130">Request</span></span>

<span data-ttu-id="ff6f3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff6f3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff6f3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="ff6f3-133">C#</span><span class="sxs-lookup"><span data-stu-id="ff6f3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff6f3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff6f3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff6f3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff6f3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ff6f3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff6f3-136">Response</span></span>

<span data-ttu-id="ff6f3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff6f3-137">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
