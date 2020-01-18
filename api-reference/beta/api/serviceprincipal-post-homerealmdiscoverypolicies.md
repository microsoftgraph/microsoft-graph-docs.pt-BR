---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribua um homeRealmDiscoveryPolicy a uma entidade de serviço.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dc108cc341af70112316f5297d12f8fab871bc3
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234099"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="07e02-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="07e02-103">Assign homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e02-104">Atribua um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="07e02-104">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="07e02-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="07e02-105">Permissions</span></span>

<span data-ttu-id="07e02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07e02-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07e02-108">Permission type</span></span>                        | <span data-ttu-id="07e02-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07e02-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="07e02-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07e02-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="07e02-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="07e02-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="07e02-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07e02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07e02-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07e02-113">Not supported.</span></span> |
| <span data-ttu-id="07e02-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07e02-114">Application</span></span>                            | <span data-ttu-id="07e02-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="07e02-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07e02-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07e02-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="07e02-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07e02-117">Request headers</span></span>

| <span data-ttu-id="07e02-118">Nome</span><span class="sxs-lookup"><span data-stu-id="07e02-118">Name</span></span>          | <span data-ttu-id="07e02-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="07e02-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="07e02-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="07e02-120">Authorization</span></span> | <span data-ttu-id="07e02-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="07e02-121">Bearer {token}</span></span> |
| <span data-ttu-id="07e02-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07e02-122">Content-Type</span></span> | <span data-ttu-id="07e02-123">application/json</span><span class="sxs-lookup"><span data-stu-id="07e02-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="07e02-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07e02-124">Request body</span></span>

<span data-ttu-id="07e02-125">No corpo da solicitação, forneça o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="07e02-125">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="07e02-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="07e02-126">Response</span></span>

<span data-ttu-id="07e02-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07e02-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07e02-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07e02-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07e02-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07e02-130">Request</span></span>

<span data-ttu-id="07e02-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07e02-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="07e02-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="07e02-132">Response</span></span>

<span data-ttu-id="07e02-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="07e02-133">The following is an example of the response.</span></span>

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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->