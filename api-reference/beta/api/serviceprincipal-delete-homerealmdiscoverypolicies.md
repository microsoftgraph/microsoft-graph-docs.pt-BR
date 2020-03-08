---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6e1a0c0568fbb72d26b7e51e731fa66301d6cec
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562728"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="1cc24-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1cc24-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="1cc24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc24-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1cc24-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc24-106">Permissions</span></span>

<span data-ttu-id="1cc24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc24-109">Permission type</span></span>                        | <span data-ttu-id="1cc24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1cc24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cc24-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1cc24-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="1cc24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc24-114">Not supported.</span></span> |
| <span data-ttu-id="1cc24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc24-115">Application</span></span>                            | <span data-ttu-id="1cc24-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1cc24-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="1cc24-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc24-118">Request headers</span></span>

| <span data-ttu-id="1cc24-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc24-119">Name</span></span>          | <span data-ttu-id="1cc24-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc24-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1cc24-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cc24-121">Authorization</span></span> | <span data-ttu-id="1cc24-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1cc24-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc24-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc24-123">Request body</span></span>

<span data-ttu-id="1cc24-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cc24-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc24-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc24-125">Response</span></span>

<span data-ttu-id="1cc24-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1cc24-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc24-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cc24-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cc24-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc24-128">Request</span></span>

<span data-ttu-id="1cc24-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc24-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="1cc24-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc24-130">Response</span></span>

<span data-ttu-id="1cc24-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc24-131">The following is an example of the response.</span></span>

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