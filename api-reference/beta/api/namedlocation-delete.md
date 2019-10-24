---
title: Excluir namedLocation
description: Excluir um objeto namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53b935349e1408bddbef291869a036bf7018b8eb
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653682"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="38411-103">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="38411-103">Delete namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38411-104">Excluir um objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="38411-104">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38411-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38411-105">Permissions</span></span>

<span data-ttu-id="38411-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38411-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38411-108">Permission type</span></span>                        | <span data-ttu-id="38411-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38411-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38411-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38411-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38411-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="38411-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="38411-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38411-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38411-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38411-113">Not supported.</span></span> |
| <span data-ttu-id="38411-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38411-114">Application</span></span>                            | <span data-ttu-id="38411-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38411-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="38411-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="38411-116">This API requires multiple permissions.</span></span> <span data-ttu-id="38411-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="38411-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="38411-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38411-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38411-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38411-119">Request headers</span></span>

| <span data-ttu-id="38411-120">Nome</span><span class="sxs-lookup"><span data-stu-id="38411-120">Name</span></span>          | <span data-ttu-id="38411-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38411-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="38411-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38411-122">Authorization</span></span> | <span data-ttu-id="38411-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38411-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38411-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38411-125">Request body</span></span>

<span data-ttu-id="38411-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38411-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38411-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="38411-127">Response</span></span>

<span data-ttu-id="38411-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38411-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38411-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38411-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38411-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38411-131">Request</span></span>

<span data-ttu-id="38411-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38411-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="38411-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38411-133">Response</span></span>

<span data-ttu-id="38411-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38411-134">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
