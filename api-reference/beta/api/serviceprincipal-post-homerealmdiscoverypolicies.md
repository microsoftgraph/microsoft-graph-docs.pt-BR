---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribuir um homeRealmDiscoveryPolicy a uma entidade de serviço.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 244b86ec441a64e5e58ef593eae332c10c2b3c6d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134180"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="2d674-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2d674-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="2d674-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d674-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d674-105">Atribuir um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a [um servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2d674-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d674-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d674-106">Permissions</span></span>

<span data-ttu-id="2d674-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d674-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d674-109">Permission type</span></span>                        | <span data-ttu-id="2d674-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d674-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d674-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d674-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d674-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d674-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="2d674-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d674-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d674-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d674-114">Not supported.</span></span> |
| <span data-ttu-id="2d674-115">Application</span><span class="sxs-lookup"><span data-stu-id="2d674-115">Application</span></span>                            | <span data-ttu-id="2d674-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d674-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d674-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d674-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2d674-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d674-118">Request headers</span></span>

| <span data-ttu-id="2d674-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2d674-119">Name</span></span>          | <span data-ttu-id="2d674-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d674-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2d674-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d674-121">Authorization</span></span> | <span data-ttu-id="2d674-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2d674-122">Bearer {token}</span></span> |
| <span data-ttu-id="2d674-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d674-123">Content-Type</span></span> | <span data-ttu-id="2d674-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d674-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d674-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d674-125">Request body</span></span>

<span data-ttu-id="2d674-126">No corpo da solicitação, fornece o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma propriedade) que deve ser atribuído à `@odata.id` entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="2d674-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="2d674-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d674-127">Response</span></span>

<span data-ttu-id="2d674-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d674-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d674-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2d674-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d674-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d674-131">Request</span></span>

<span data-ttu-id="2d674-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d674-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d674-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d674-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2d674-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d674-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2d674-135">C#</span><span class="sxs-lookup"><span data-stu-id="2d674-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d674-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d674-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d674-137">Java</span><span class="sxs-lookup"><span data-stu-id="2d674-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d674-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d674-138">Response</span></span>

<span data-ttu-id="2d674-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d674-139">The following is an example of the response.</span></span>

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



