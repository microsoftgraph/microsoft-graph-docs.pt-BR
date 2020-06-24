---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8c5f152f8e44f31b0016b480019fb36d132d953
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846189"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="fcb55-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="fcb55-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="fcb55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcb55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcb55-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="fcb55-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fcb55-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcb55-106">Permissions</span></span>

<span data-ttu-id="fcb55-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fcb55-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fcb55-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcb55-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fcb55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcb55-109">Permission type</span></span>                        | <span data-ttu-id="fcb55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcb55-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fcb55-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcb55-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fcb55-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fcb55-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="fcb55-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcb55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcb55-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcb55-114">Not supported.</span></span> |
| <span data-ttu-id="fcb55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcb55-115">Application</span></span>                            | <span data-ttu-id="fcb55-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fcb55-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcb55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcb55-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fcb55-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb55-118">Request headers</span></span>

| <span data-ttu-id="fcb55-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fcb55-119">Name</span></span>          | <span data-ttu-id="fcb55-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb55-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fcb55-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcb55-121">Authorization</span></span> | <span data-ttu-id="fcb55-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="fcb55-122">Bearer {token}.</span></span> <span data-ttu-id="fcb55-123">Required.</span><span class="sxs-lookup"><span data-stu-id="fcb55-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcb55-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb55-124">Request body</span></span>

<span data-ttu-id="fcb55-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcb55-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcb55-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcb55-126">Response</span></span>

<span data-ttu-id="fcb55-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fcb55-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fcb55-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fcb55-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fcb55-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcb55-129">Request</span></span>

<span data-ttu-id="fcb55-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcb55-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcb55-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcb55-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="fcb55-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcb55-132">Response</span></span>

<span data-ttu-id="fcb55-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcb55-133">The following is an example of the response.</span></span>

> <span data-ttu-id="fcb55-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="fcb55-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fcb55-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fcb55-135">All the properties will be returned from an actual call.</span></span>

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
