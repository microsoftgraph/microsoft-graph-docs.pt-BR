---
title: Excluir countryNamedLocation
description: Excluir um objeto countryNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f56ed6245102cfe01744f22ca0a36fa22d5c4df
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653696"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="088a6-103">Excluir countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="088a6-103">Delete countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="088a6-104">Excluir um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="088a6-104">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="088a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="088a6-105">Permissions</span></span>

<span data-ttu-id="088a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="088a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="088a6-108">Permission type</span></span>                        | <span data-ttu-id="088a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="088a6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="088a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="088a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="088a6-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="088a6-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="088a6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="088a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="088a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088a6-113">Not supported.</span></span> |
| <span data-ttu-id="088a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="088a6-114">Application</span></span>                            | <span data-ttu-id="088a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088a6-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="088a6-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="088a6-116">This API requires multiple permissions.</span></span> <span data-ttu-id="088a6-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="088a6-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="088a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="088a6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="088a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="088a6-119">Request headers</span></span>

| <span data-ttu-id="088a6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="088a6-120">Name</span></span>          | <span data-ttu-id="088a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="088a6-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="088a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="088a6-122">Authorization</span></span> | <span data-ttu-id="088a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="088a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="088a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="088a6-125">Request body</span></span>

<span data-ttu-id="088a6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="088a6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="088a6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="088a6-127">Response</span></span>

<span data-ttu-id="088a6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="088a6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="088a6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="088a6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="088a6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="088a6-131">Request</span></span>

<span data-ttu-id="088a6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="088a6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```

### <a name="response"></a><span data-ttu-id="088a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="088a6-133">Response</span></span>

<span data-ttu-id="088a6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="088a6-134">The following is an example of the response.</span></span>

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
