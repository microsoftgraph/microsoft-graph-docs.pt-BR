---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 421fb9be650ab22c07e940ab2eac2fcf20abf5a7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234110"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="57a1b-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="57a1b-103">Remove homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57a1b-104">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="57a1b-104">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57a1b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="57a1b-105">Permissions</span></span>

<span data-ttu-id="57a1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57a1b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a1b-108">Permission type</span></span>                        | <span data-ttu-id="57a1b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57a1b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57a1b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a1b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="57a1b-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57a1b-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="57a1b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57a1b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a1b-113">Not supported.</span></span> |
| <span data-ttu-id="57a1b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a1b-114">Application</span></span>                            | <span data-ttu-id="57a1b-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57a1b-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57a1b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a1b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="57a1b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57a1b-117">Request headers</span></span>

| <span data-ttu-id="57a1b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="57a1b-118">Name</span></span>          | <span data-ttu-id="57a1b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="57a1b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="57a1b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="57a1b-120">Authorization</span></span> | <span data-ttu-id="57a1b-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="57a1b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57a1b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57a1b-122">Request body</span></span>

<span data-ttu-id="57a1b-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57a1b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57a1b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a1b-124">Response</span></span>

<span data-ttu-id="57a1b-125">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57a1b-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="57a1b-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57a1b-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57a1b-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a1b-127">Request</span></span>

<span data-ttu-id="57a1b-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57a1b-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="57a1b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a1b-129">Response</span></span>

<span data-ttu-id="57a1b-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57a1b-130">The following is an example of the response.</span></span>

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