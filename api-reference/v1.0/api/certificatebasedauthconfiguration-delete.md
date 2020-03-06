---
title: Excluir certificateBasedAuthConfiguration
description: Exclua certificateBasedAuthConfiguration.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a09ab17568e539ccce87c50d5d8c5180e0c30334
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518641"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="0601f-103">Excluir certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="0601f-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="0601f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0601f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0601f-105">Excluir um objeto [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0601f-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0601f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0601f-106">Permissions</span></span>

<span data-ttu-id="0601f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0601f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0601f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0601f-109">Permission type</span></span>                        | <span data-ttu-id="0601f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0601f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0601f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0601f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0601f-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0601f-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="0601f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0601f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0601f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0601f-114">Not supported.</span></span> |
| <span data-ttu-id="0601f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0601f-115">Application</span></span>    | <span data-ttu-id="0601f-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0601f-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0601f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0601f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0601f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0601f-118">Request headers</span></span>

| <span data-ttu-id="0601f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0601f-119">Name</span></span>          | <span data-ttu-id="0601f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0601f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0601f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0601f-121">Authorization</span></span> | <span data-ttu-id="0601f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0601f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0601f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0601f-124">Request body</span></span>

<span data-ttu-id="0601f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0601f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0601f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0601f-126">Response</span></span>

<span data-ttu-id="0601f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0601f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0601f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0601f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0601f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0601f-130">Request</span></span>

<span data-ttu-id="0601f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0601f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0601f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0601f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="0601f-133">C#</span><span class="sxs-lookup"><span data-stu-id="0601f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0601f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0601f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0601f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0601f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0601f-136">Java</span><span class="sxs-lookup"><span data-stu-id="0601f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0601f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0601f-137">Response</span></span>

<span data-ttu-id="0601f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0601f-138">The following is an example of the response.</span></span>

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
