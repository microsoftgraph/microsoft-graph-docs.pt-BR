---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b404a68afd042e20a5c0b43ebd4ca1faf0287685
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437850"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="60319-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="60319-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="60319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60319-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60319-105">[Exclua um objeto certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60319-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60319-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60319-106">Permissions</span></span>

<span data-ttu-id="60319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60319-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60319-109">Permission type</span></span>                        | <span data-ttu-id="60319-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60319-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60319-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60319-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60319-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60319-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="60319-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60319-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60319-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60319-114">Not supported.</span></span> |
| <span data-ttu-id="60319-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60319-115">Application</span></span>    | <span data-ttu-id="60319-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60319-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60319-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60319-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60319-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60319-118">Request headers</span></span>

| <span data-ttu-id="60319-119">Nome</span><span class="sxs-lookup"><span data-stu-id="60319-119">Name</span></span>          | <span data-ttu-id="60319-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="60319-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60319-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="60319-121">Authorization</span></span> | <span data-ttu-id="60319-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="60319-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60319-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60319-123">Request body</span></span>

<span data-ttu-id="60319-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60319-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60319-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="60319-125">Response</span></span>

<span data-ttu-id="60319-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60319-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60319-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60319-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60319-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60319-129">Request</span></span>

<span data-ttu-id="60319-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60319-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60319-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="60319-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="60319-132">C#</span><span class="sxs-lookup"><span data-stu-id="60319-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60319-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60319-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60319-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60319-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60319-135">Java</span><span class="sxs-lookup"><span data-stu-id="60319-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60319-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="60319-136">Response</span></span>

<span data-ttu-id="60319-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60319-137">The following is an example of the response.</span></span>

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


