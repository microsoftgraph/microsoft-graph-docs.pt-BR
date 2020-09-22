---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribua um homeRealmDiscoveryPolicy a uma entidade de serviço.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1991e21b5dc1c6c0b2ced2904a17b65257e7a5dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076761"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="b58f4-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b58f4-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="b58f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b58f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58f4-105">Atribua um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b58f4-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b58f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b58f4-106">Permissions</span></span>

<span data-ttu-id="b58f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b58f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b58f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b58f4-109">Permission type</span></span>                        | <span data-ttu-id="b58f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b58f4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b58f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b58f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b58f4-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b58f4-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="b58f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b58f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b58f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b58f4-114">Not supported.</span></span> |
| <span data-ttu-id="b58f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b58f4-115">Application</span></span>                            | <span data-ttu-id="b58f4-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b58f4-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b58f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b58f4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b58f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b58f4-118">Request headers</span></span>

| <span data-ttu-id="b58f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b58f4-119">Name</span></span>          | <span data-ttu-id="b58f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b58f4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b58f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b58f4-121">Authorization</span></span> | <span data-ttu-id="b58f4-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b58f4-122">Bearer {token}</span></span> |
| <span data-ttu-id="b58f4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b58f4-123">Content-Type</span></span> | <span data-ttu-id="b58f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b58f4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b58f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b58f4-125">Request body</span></span>

<span data-ttu-id="b58f4-126">No corpo da solicitação, forneça o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="b58f4-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="b58f4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b58f4-127">Response</span></span>

<span data-ttu-id="b58f4-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b58f4-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b58f4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b58f4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b58f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b58f4-131">Request</span></span>

<span data-ttu-id="b58f4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b58f4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b58f4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b58f4-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b58f4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b58f4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b58f4-135">C#</span><span class="sxs-lookup"><span data-stu-id="b58f4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b58f4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b58f4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b58f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b58f4-137">Response</span></span>

<span data-ttu-id="b58f4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b58f4-138">The following is an example of the response.</span></span>

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


