---
title: Atribuir claimsMappingPolicy
description: Atribua um claimsMappingPolicy a uma entidade de serviço.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fea8527d6da5f9422e1d81c5f2a0a662dfcd00c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453363"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="7023a-103">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="7023a-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="7023a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7023a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7023a-105">Atribua um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="7023a-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7023a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7023a-106">Permissions</span></span>

<span data-ttu-id="7023a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7023a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7023a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7023a-109">Permission type</span></span>                        | <span data-ttu-id="7023a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7023a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7023a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7023a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7023a-112">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7023a-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="7023a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7023a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7023a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7023a-114">Not supported.</span></span> |
| <span data-ttu-id="7023a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7023a-115">Application</span></span>                            | <span data-ttu-id="7023a-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7023a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7023a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7023a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7023a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7023a-118">Request headers</span></span>

| <span data-ttu-id="7023a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7023a-119">Name</span></span>          | <span data-ttu-id="7023a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7023a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7023a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7023a-121">Authorization</span></span> | <span data-ttu-id="7023a-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="7023a-122">Bearer {token}</span></span> |
| <span data-ttu-id="7023a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7023a-123">Content-Type</span></span> | <span data-ttu-id="7023a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7023a-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7023a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7023a-125">Request body</span></span>

<span data-ttu-id="7023a-126">No corpo da solicitação, forneça o identificador do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="7023a-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="7023a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7023a-127">Response</span></span>

<span data-ttu-id="7023a-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7023a-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7023a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7023a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7023a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7023a-131">Request</span></span>

<span data-ttu-id="7023a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7023a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7023a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7023a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7023a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7023a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7023a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7023a-135">Response</span></span>

<span data-ttu-id="7023a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7023a-136">The following is an example of the response.</span></span>

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
  "description": "Assign claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
