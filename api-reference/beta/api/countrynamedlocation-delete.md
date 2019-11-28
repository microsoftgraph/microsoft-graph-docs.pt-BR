---
title: Excluir countryNamedLocation
description: Excluir um objeto countryNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20b3058f46811edebe4fcf468f1156bf47971700
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636789"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="02b7a-103">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="02b7a-103">Delete countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02b7a-104">Excluir um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="02b7a-104">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02b7a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02b7a-105">Permissions</span></span>

<span data-ttu-id="02b7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02b7a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02b7a-108">Permission type</span></span>                        | <span data-ttu-id="02b7a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02b7a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02b7a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02b7a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02b7a-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="02b7a-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="02b7a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02b7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02b7a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02b7a-113">Not supported.</span></span> |
| <span data-ttu-id="02b7a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02b7a-114">Application</span></span>                            | <span data-ttu-id="02b7a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02b7a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02b7a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02b7a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="02b7a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02b7a-117">Request headers</span></span>

| <span data-ttu-id="02b7a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02b7a-118">Name</span></span>          | <span data-ttu-id="02b7a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02b7a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="02b7a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02b7a-120">Authorization</span></span> | <span data-ttu-id="02b7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02b7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02b7a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02b7a-123">Request body</span></span>

<span data-ttu-id="02b7a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02b7a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02b7a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b7a-125">Response</span></span>

<span data-ttu-id="02b7a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02b7a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02b7a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02b7a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02b7a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02b7a-129">Request</span></span>

<span data-ttu-id="02b7a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02b7a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02b7a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="02b7a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02b7a-132">C#</span><span class="sxs-lookup"><span data-stu-id="02b7a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02b7a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02b7a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02b7a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02b7a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02b7a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="02b7a-135">Response</span></span>

<span data-ttu-id="02b7a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02b7a-136">The following is an example of the response.</span></span>

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
