---
title: Excluir countryNamedLocation
description: Excluir um objeto countryNamedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ffce6907d9591ebe3ef6516c54ff97b4939201c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002671"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="0db5c-103">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="0db5c-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="0db5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db5c-105">Excluir um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="0db5c-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0db5c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0db5c-106">Permissions</span></span>

<span data-ttu-id="0db5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0db5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0db5c-109">Permission type</span></span>                        | <span data-ttu-id="0db5c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0db5c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0db5c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0db5c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0db5c-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="0db5c-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="0db5c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0db5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0db5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0db5c-114">Not supported.</span></span> |
| <span data-ttu-id="0db5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0db5c-115">Application</span></span>                            | <span data-ttu-id="0db5c-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="0db5c-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="0db5c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0db5c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0db5c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0db5c-118">Request headers</span></span>

| <span data-ttu-id="0db5c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0db5c-119">Name</span></span>          | <span data-ttu-id="0db5c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db5c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0db5c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0db5c-121">Authorization</span></span> | <span data-ttu-id="0db5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0db5c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0db5c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0db5c-124">Request body</span></span>

<span data-ttu-id="0db5c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0db5c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0db5c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db5c-126">Response</span></span>

<span data-ttu-id="0db5c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0db5c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0db5c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0db5c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0db5c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0db5c-130">Request</span></span>

<span data-ttu-id="0db5c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0db5c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0db5c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0db5c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="0db5c-133">C#</span><span class="sxs-lookup"><span data-stu-id="0db5c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0db5c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0db5c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0db5c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0db5c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0db5c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db5c-136">Response</span></span>

<span data-ttu-id="0db5c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0db5c-137">The following is an example of the response.</span></span>

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
  "description": "Delete countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


