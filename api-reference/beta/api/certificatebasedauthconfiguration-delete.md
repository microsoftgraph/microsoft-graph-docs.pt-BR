---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce54ddecbaa166a64ba5379c09729af44baad7d8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718716"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="fae23-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="fae23-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae23-104">Excluir um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fae23-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fae23-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fae23-105">Permissions</span></span>

<span data-ttu-id="fae23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fae23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fae23-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fae23-108">Permission type</span></span>                        | <span data-ttu-id="fae23-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fae23-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fae23-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fae23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fae23-111">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fae23-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="fae23-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fae23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fae23-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fae23-113">Not supported.</span></span> |
| <span data-ttu-id="fae23-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fae23-114">Application</span></span>    | <span data-ttu-id="fae23-115">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fae23-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fae23-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fae23-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fae23-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fae23-117">Request headers</span></span>

| <span data-ttu-id="fae23-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fae23-118">Name</span></span>          | <span data-ttu-id="fae23-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fae23-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fae23-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fae23-120">Authorization</span></span> | <span data-ttu-id="fae23-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="fae23-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae23-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fae23-122">Request body</span></span>

<span data-ttu-id="fae23-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fae23-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae23-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="fae23-124">Response</span></span>

<span data-ttu-id="fae23-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fae23-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fae23-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fae23-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fae23-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fae23-128">Request</span></span>

<span data-ttu-id="fae23-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fae23-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fae23-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fae23-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fae23-131">C#</span><span class="sxs-lookup"><span data-stu-id="fae23-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fae23-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fae23-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fae23-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fae23-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fae23-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fae23-134">Response</span></span>

<span data-ttu-id="fae23-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fae23-135">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
