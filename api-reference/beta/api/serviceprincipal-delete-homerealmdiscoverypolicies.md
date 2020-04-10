---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fce52e77c38bddf446819b81c638d9234c8f9c7f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219309"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="f9e58-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="f9e58-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="f9e58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9e58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9e58-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f9e58-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9e58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9e58-106">Permissions</span></span>

<span data-ttu-id="f9e58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9e58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9e58-109">Permission type</span></span>                        | <span data-ttu-id="f9e58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9e58-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9e58-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9e58-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9e58-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f9e58-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="f9e58-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9e58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9e58-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9e58-114">Not supported.</span></span> |
| <span data-ttu-id="f9e58-115">Application</span><span class="sxs-lookup"><span data-stu-id="f9e58-115">Application</span></span>                            | <span data-ttu-id="f9e58-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f9e58-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9e58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9e58-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="f9e58-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e58-118">Request headers</span></span>

| <span data-ttu-id="f9e58-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f9e58-119">Name</span></span>          | <span data-ttu-id="f9e58-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e58-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f9e58-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9e58-121">Authorization</span></span> | <span data-ttu-id="f9e58-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f9e58-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9e58-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e58-123">Request body</span></span>

<span data-ttu-id="f9e58-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9e58-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9e58-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e58-125">Response</span></span>

<span data-ttu-id="f9e58-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9e58-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f9e58-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9e58-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9e58-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9e58-128">Request</span></span>

<span data-ttu-id="f9e58-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9e58-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9e58-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9e58-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f9e58-131">C#</span><span class="sxs-lookup"><span data-stu-id="f9e58-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9e58-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9e58-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9e58-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9e58-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9e58-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9e58-134">Response</span></span>

<span data-ttu-id="f9e58-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9e58-135">The following is an example of the response.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
