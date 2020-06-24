---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribua um homeRealmDiscoveryPolicy a um servicePrincipalName.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387c8a1535ed040040475ef5c0c2e9a7d6cbb258
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846208"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="9c101-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="9c101-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="9c101-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c101-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="9c101-105">Atribua um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="9c101-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c101-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c101-106">Permissions</span></span>

<span data-ttu-id="9c101-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9c101-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9c101-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c101-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c101-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c101-109">Permission type</span></span>                        | <span data-ttu-id="9c101-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c101-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9c101-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c101-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c101-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9c101-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="9c101-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c101-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c101-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c101-114">Not supported.</span></span> |
| <span data-ttu-id="9c101-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c101-115">Application</span></span>                            | <span data-ttu-id="9c101-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9c101-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c101-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c101-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9c101-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c101-118">Request headers</span></span>

| <span data-ttu-id="9c101-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9c101-119">Name</span></span>          | <span data-ttu-id="9c101-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c101-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9c101-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c101-121">Authorization</span></span> | <span data-ttu-id="9c101-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="9c101-122">Bearer {token}.</span></span> <span data-ttu-id="9c101-123">Required.</span><span class="sxs-lookup"><span data-stu-id="9c101-123">Required.</span></span> |
| <span data-ttu-id="9c101-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c101-124">Content-Type</span></span> | <span data-ttu-id="9c101-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="9c101-125">application/json.</span></span> <span data-ttu-id="9c101-126">Required.</span><span class="sxs-lookup"><span data-stu-id="9c101-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c101-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c101-127">Request body</span></span>

<span data-ttu-id="9c101-128">No corpo da solicitação, forneça o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="9c101-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="9c101-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c101-129">Response</span></span>

<span data-ttu-id="9c101-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="9c101-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="9c101-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="9c101-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c101-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c101-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c101-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c101-133">Request</span></span>

<span data-ttu-id="9c101-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c101-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c101-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c101-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="9c101-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c101-136">Response</span></span>

<span data-ttu-id="9c101-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c101-137">The following is an example of the response.</span></span>

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
