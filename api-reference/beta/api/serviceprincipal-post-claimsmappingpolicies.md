---
title: Atribuir claimsMappingPolicy
description: Atribua um claimsMappingPolicy a uma entidade de serviço.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fca74b192ac261edbe4ba0e6af67760d409dd30d
ms.sourcegitcommit: c6e8a2097267ace4c78124be48646f9129114b26
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47340037"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="b0c28-103">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="b0c28-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="b0c28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c28-105">Atribua um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b0c28-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0c28-106">Permissions</span></span>

<span data-ttu-id="b0c28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0c28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0c28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0c28-109">Permission type</span></span>                        | <span data-ttu-id="b0c28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0c28-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0c28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0c28-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0c28-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b0c28-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="b0c28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0c28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c28-114">Not supported.</span></span> |
| <span data-ttu-id="b0c28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0c28-115">Application</span></span>                            | <span data-ttu-id="b0c28-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b0c28-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0c28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c28-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b0c28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c28-118">Request headers</span></span>

| <span data-ttu-id="b0c28-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b0c28-119">Name</span></span>          | <span data-ttu-id="b0c28-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c28-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b0c28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0c28-121">Authorization</span></span> | <span data-ttu-id="b0c28-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b0c28-122">Bearer {token}</span></span> |
| <span data-ttu-id="b0c28-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0c28-123">Content-Type</span></span> | <span data-ttu-id="b0c28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0c28-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0c28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c28-125">Request body</span></span>

<span data-ttu-id="b0c28-126">No corpo da solicitação, forneça o identificador do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="b0c28-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="b0c28-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c28-127">Response</span></span>

<span data-ttu-id="b0c28-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c28-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0c28-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b0c28-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0c28-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c28-131">Request</span></span>

<span data-ttu-id="b0c28-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0c28-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0c28-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c28-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="b0c28-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0c28-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b0c28-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0c28-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0c28-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0c28-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0c28-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c28-137">Response</span></span>

<span data-ttu-id="b0c28-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c28-138">The following is an example of the response.</span></span>

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
