---
title: Excluir accessPackageCatalog
description: Exclua accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02de5e5ac3f6b5caa96e6dcad77522d3b92dcce1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983785"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="1025a-103">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1025a-103">Delete accessPackageCatalog</span></span>

<span data-ttu-id="1025a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1025a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1025a-105">Excluir um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="1025a-105">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1025a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1025a-106">Permissions</span></span>

<span data-ttu-id="1025a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1025a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1025a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1025a-109">Permission type</span></span>                        | <span data-ttu-id="1025a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1025a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1025a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1025a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1025a-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1025a-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1025a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1025a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1025a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1025a-114">Not supported.</span></span> |
| <span data-ttu-id="1025a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1025a-115">Application</span></span>                            | <span data-ttu-id="1025a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1025a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1025a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1025a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1025a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1025a-118">Request headers</span></span>

| <span data-ttu-id="1025a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1025a-119">Name</span></span>          | <span data-ttu-id="1025a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1025a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1025a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1025a-121">Authorization</span></span> | <span data-ttu-id="1025a-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1025a-122">Bearer \{token\}.</span></span> <span data-ttu-id="1025a-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1025a-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1025a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1025a-124">Request body</span></span>

<span data-ttu-id="1025a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1025a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1025a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1025a-126">Response</span></span>

<span data-ttu-id="1025a-127">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="1025a-127">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="1025a-128">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1025a-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1025a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1025a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1025a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1025a-130">Request</span></span>

<span data-ttu-id="1025a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1025a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1025a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1025a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="1025a-133">C#</span><span class="sxs-lookup"><span data-stu-id="1025a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1025a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1025a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1025a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1025a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1025a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1025a-136">Response</span></span>

<span data-ttu-id="1025a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1025a-137">The following is an example of the response.</span></span>

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


