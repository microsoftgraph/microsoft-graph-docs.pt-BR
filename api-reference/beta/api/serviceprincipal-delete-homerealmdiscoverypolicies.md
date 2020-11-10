---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa704fcd0bd997fe2880183ebc03bf75c3ebf0a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969657"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="68bfd-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="68bfd-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="68bfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68bfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68bfd-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="68bfd-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68bfd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68bfd-106">Permissions</span></span>

<span data-ttu-id="68bfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68bfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68bfd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68bfd-109">Permission type</span></span>                        | <span data-ttu-id="68bfd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68bfd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68bfd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68bfd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68bfd-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68bfd-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="68bfd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68bfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68bfd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68bfd-114">Not supported.</span></span> |
| <span data-ttu-id="68bfd-115">Application</span><span class="sxs-lookup"><span data-stu-id="68bfd-115">Application</span></span>                            | <span data-ttu-id="68bfd-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68bfd-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68bfd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68bfd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="68bfd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-118">Request headers</span></span>

| <span data-ttu-id="68bfd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="68bfd-119">Name</span></span>          | <span data-ttu-id="68bfd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68bfd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68bfd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68bfd-121">Authorization</span></span> | <span data-ttu-id="68bfd-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="68bfd-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="68bfd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-123">Request body</span></span>

<span data-ttu-id="68bfd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68bfd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68bfd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="68bfd-125">Response</span></span>

<span data-ttu-id="68bfd-126">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68bfd-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="68bfd-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68bfd-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68bfd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-128">Request</span></span>

<span data-ttu-id="68bfd-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68bfd-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68bfd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="68bfd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="68bfd-131">C#</span><span class="sxs-lookup"><span data-stu-id="68bfd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68bfd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68bfd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68bfd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68bfd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68bfd-134">Java</span><span class="sxs-lookup"><span data-stu-id="68bfd-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68bfd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="68bfd-135">Response</span></span>

<span data-ttu-id="68bfd-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-136">The following is an example of the response.</span></span>

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


