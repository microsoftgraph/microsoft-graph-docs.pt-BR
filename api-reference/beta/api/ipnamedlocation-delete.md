---
title: Excluir ipNamedLocation
description: Excluir um objeto ipNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6ba92dc18fce372d963a450798e3037b078963d6
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062307"
---
# <a name="delete-ipnamedlocation"></a><span data-ttu-id="be88d-103">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be88d-103">Delete ipNamedLocation</span></span>

<span data-ttu-id="be88d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be88d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be88d-105">Excluir um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="be88d-105">Delete an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be88d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be88d-106">Permissions</span></span>

<span data-ttu-id="be88d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be88d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be88d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be88d-109">Permission type</span></span>                        | <span data-ttu-id="be88d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be88d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be88d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be88d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be88d-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="be88d-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="be88d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be88d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be88d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be88d-114">Not supported.</span></span> |
| <span data-ttu-id="be88d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be88d-115">Application</span></span>                            | <span data-ttu-id="be88d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be88d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be88d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be88d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="be88d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be88d-118">Request headers</span></span>

| <span data-ttu-id="be88d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="be88d-119">Name</span></span>          | <span data-ttu-id="be88d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="be88d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be88d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be88d-121">Authorization</span></span> | <span data-ttu-id="be88d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be88d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be88d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be88d-124">Request body</span></span>

<span data-ttu-id="be88d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be88d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be88d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="be88d-126">Response</span></span>

<span data-ttu-id="be88d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be88d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be88d-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be88d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be88d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be88d-130">Request</span></span>

<span data-ttu-id="be88d-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be88d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be88d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="be88d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ipnamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="be88d-133">C#</span><span class="sxs-lookup"><span data-stu-id="be88d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be88d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be88d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be88d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be88d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be88d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="be88d-136">Response</span></span>

<span data-ttu-id="be88d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be88d-137">The following is an example of the response.</span></span>

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
  "description": "Delete ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
