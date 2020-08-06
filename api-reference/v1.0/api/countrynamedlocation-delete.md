---
title: Excluir countryNamedLocation
description: Excluir um objeto countryNamedLocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f72caeb1c181b58380dd8fea2d816b0cc6d3314
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567157"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="7b61f-103">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="7b61f-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="7b61f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b61f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b61f-105">Excluir um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="7b61f-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b61f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b61f-106">Permissions</span></span>

<span data-ttu-id="7b61f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b61f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b61f-109">Permission type</span></span>                        | <span data-ttu-id="7b61f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b61f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b61f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b61f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b61f-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="7b61f-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="7b61f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b61f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b61f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b61f-114">Not supported.</span></span> |
| <span data-ttu-id="7b61f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b61f-115">Application</span></span>                            | <span data-ttu-id="7b61f-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="7b61f-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b61f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b61f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b61f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b61f-118">Request headers</span></span>

| <span data-ttu-id="7b61f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7b61f-119">Name</span></span>          | <span data-ttu-id="7b61f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b61f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b61f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b61f-121">Authorization</span></span> | <span data-ttu-id="7b61f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b61f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b61f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b61f-124">Request body</span></span>

<span data-ttu-id="7b61f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b61f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b61f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b61f-126">Response</span></span>

<span data-ttu-id="7b61f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b61f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b61f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b61f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b61f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b61f-130">Request</span></span>

<span data-ttu-id="7b61f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b61f-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b61f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b61f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="7b61f-133">C#</span><span class="sxs-lookup"><span data-stu-id="7b61f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b61f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b61f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b61f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b61f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b61f-136">Java</span><span class="sxs-lookup"><span data-stu-id="7b61f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b61f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b61f-137">Response</span></span>

<span data-ttu-id="7b61f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b61f-138">The following is an example of the response.</span></span>

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
