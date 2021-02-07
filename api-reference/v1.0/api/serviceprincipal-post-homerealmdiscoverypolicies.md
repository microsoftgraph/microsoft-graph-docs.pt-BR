---
title: Atribuir homeRealmDiscoveryPolicy
description: Atribua um homeRealmDiscoveryPolicy a uma servicePrincipal.
localization_priority: Normal
author: hpsin
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8a361503ad29fbaf4fae198b3c3843f07d0fc5fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128698"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="d015d-103">Atribuir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d015d-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="d015d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d015d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d015d-105">Atribuir um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) a [um servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="d015d-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d015d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d015d-106">Permissions</span></span>

<span data-ttu-id="d015d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d015d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d015d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d015d-109">Permission type</span></span>                        | <span data-ttu-id="d015d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d015d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d015d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d015d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d015d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d015d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="d015d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d015d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d015d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d015d-114">Not supported.</span></span> |
| <span data-ttu-id="d015d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d015d-115">Application</span></span>                            | <span data-ttu-id="d015d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d015d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d015d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d015d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d015d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d015d-118">Request headers</span></span>

| <span data-ttu-id="d015d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d015d-119">Name</span></span>          | <span data-ttu-id="d015d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d015d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d015d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d015d-121">Authorization</span></span> | <span data-ttu-id="d015d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d015d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d015d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d015d-124">Content-Type</span></span> | <span data-ttu-id="d015d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d015d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d015d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d015d-127">Request body</span></span>

<span data-ttu-id="d015d-128">No corpo da solicitação, fornece o identificador do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (usando uma propriedade) que deve ser atribuído à `@odata.id` entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="d015d-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="d015d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d015d-129">Response</span></span>

<span data-ttu-id="d015d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d015d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d015d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d015d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d015d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d015d-133">Request</span></span>

<span data-ttu-id="d015d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d015d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d015d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d015d-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d015d-136">C#</span><span class="sxs-lookup"><span data-stu-id="d015d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d015d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d015d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d015d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d015d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d015d-139">Java</span><span class="sxs-lookup"><span data-stu-id="d015d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d015d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d015d-140">Response</span></span>

<span data-ttu-id="d015d-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d015d-141">The following is an example of the response.</span></span>

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

