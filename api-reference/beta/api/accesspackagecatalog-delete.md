---
title: Excluir accessPackageCatalog
description: Exclua accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 063b2baff5ad2bae4ff9ea68e32daf689ceca6dc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994320"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="2de8e-103">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2de8e-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2de8e-104">Excluir um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="2de8e-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2de8e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2de8e-105">Permissions</span></span>

<span data-ttu-id="2de8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2de8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2de8e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2de8e-108">Permission type</span></span>                        | <span data-ttu-id="2de8e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2de8e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2de8e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2de8e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2de8e-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de8e-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="2de8e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2de8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2de8e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2de8e-113">Not supported.</span></span> |
| <span data-ttu-id="2de8e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2de8e-114">Application</span></span>                            | <span data-ttu-id="2de8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2de8e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2de8e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2de8e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2de8e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2de8e-117">Request headers</span></span>

| <span data-ttu-id="2de8e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2de8e-118">Name</span></span>          | <span data-ttu-id="2de8e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2de8e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2de8e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2de8e-120">Authorization</span></span> | <span data-ttu-id="2de8e-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="2de8e-121">Bearer \{token\}.</span></span> <span data-ttu-id="2de8e-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2de8e-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2de8e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2de8e-123">Request body</span></span>

<span data-ttu-id="2de8e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2de8e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2de8e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de8e-125">Response</span></span>

<span data-ttu-id="2de8e-126">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="2de8e-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="2de8e-127">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2de8e-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2de8e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2de8e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2de8e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2de8e-129">Request</span></span>

<span data-ttu-id="2de8e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2de8e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2de8e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2de8e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2de8e-132">C#</span><span class="sxs-lookup"><span data-stu-id="2de8e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2de8e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2de8e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2de8e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2de8e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2de8e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2de8e-135">Response</span></span>

<span data-ttu-id="2de8e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2de8e-136">The following is an example of the response.</span></span>

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
