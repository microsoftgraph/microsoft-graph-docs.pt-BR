---
title: Excluir countryNamedLocation
description: Excluir um objeto countryNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e7b7534031d392ff40379e87104ccd9dea3e8c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937151"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="9643e-103">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="9643e-103">Delete countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9643e-104">Excluir um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="9643e-104">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9643e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9643e-105">Permissions</span></span>

<span data-ttu-id="9643e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9643e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9643e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9643e-108">Permission type</span></span>                        | <span data-ttu-id="9643e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9643e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9643e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9643e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9643e-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9643e-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9643e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9643e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9643e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9643e-113">Not supported.</span></span> |
| <span data-ttu-id="9643e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9643e-114">Application</span></span>                            | <span data-ttu-id="9643e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9643e-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="9643e-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="9643e-116">This API requires multiple permissions.</span></span> <span data-ttu-id="9643e-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="9643e-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="9643e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9643e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9643e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9643e-119">Request headers</span></span>

| <span data-ttu-id="9643e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9643e-120">Name</span></span>          | <span data-ttu-id="9643e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9643e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9643e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9643e-122">Authorization</span></span> | <span data-ttu-id="9643e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9643e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9643e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9643e-125">Request body</span></span>

<span data-ttu-id="9643e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9643e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9643e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9643e-127">Response</span></span>

<span data-ttu-id="9643e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9643e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9643e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9643e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9643e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9643e-131">Request</span></span>

<span data-ttu-id="9643e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9643e-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9643e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9643e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9643e-134">C#</span><span class="sxs-lookup"><span data-stu-id="9643e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9643e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9643e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9643e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9643e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9643e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9643e-137">Response</span></span>

<span data-ttu-id="9643e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9643e-138">The following is an example of the response.</span></span>

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
