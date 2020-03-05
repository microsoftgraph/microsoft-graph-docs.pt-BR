---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribua um homeRealmDiscoveryPolicy a uma entidade de serviço.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ecd671e9ac5918c27b3b0802bb52e7deb6bad6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453356"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="68e07-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="68e07-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="68e07-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68e07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e07-105">Atribua um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="68e07-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68e07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68e07-106">Permissions</span></span>

<span data-ttu-id="68e07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68e07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68e07-109">Permission type</span></span>                        | <span data-ttu-id="68e07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68e07-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68e07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68e07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68e07-112">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68e07-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="68e07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68e07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68e07-114">Not supported.</span></span> |
| <span data-ttu-id="68e07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68e07-115">Application</span></span>                            | <span data-ttu-id="68e07-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68e07-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68e07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="68e07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68e07-118">Request headers</span></span>

| <span data-ttu-id="68e07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="68e07-119">Name</span></span>          | <span data-ttu-id="68e07-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68e07-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68e07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68e07-121">Authorization</span></span> | <span data-ttu-id="68e07-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="68e07-122">Bearer {token}</span></span> |
| <span data-ttu-id="68e07-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68e07-123">Content-Type</span></span> | <span data-ttu-id="68e07-124">application/json</span><span class="sxs-lookup"><span data-stu-id="68e07-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="68e07-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68e07-125">Request body</span></span>

<span data-ttu-id="68e07-126">No corpo da solicitação, forneça o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="68e07-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="68e07-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e07-127">Response</span></span>

<span data-ttu-id="68e07-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68e07-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68e07-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68e07-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68e07-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68e07-131">Request</span></span>

<span data-ttu-id="68e07-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68e07-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68e07-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="68e07-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="68e07-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68e07-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68e07-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="68e07-135">Response</span></span>

<span data-ttu-id="68e07-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68e07-136">The following is an example of the response.</span></span>

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
