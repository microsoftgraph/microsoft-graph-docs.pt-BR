---
title: Atribuir claimsMappingPolicy
description: Atribua um claimsMappingPolicy a uma servicePrincipal.
localization_priority: Normal
author: paulgarn
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: de92c1f75288c4e5c0575eb7369dd8d7bf1e4ce0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135790"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="83d3a-103">Atribuir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="83d3a-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="83d3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d3a-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="83d3a-105">Atribuir um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) a [um servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="83d3a-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83d3a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="83d3a-106">Permissions</span></span>

<span data-ttu-id="83d3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83d3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d3a-109">Permission type</span></span>                        | <span data-ttu-id="83d3a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83d3a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83d3a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d3a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83d3a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d3a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="83d3a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d3a-114">Not supported.</span></span> |
| <span data-ttu-id="83d3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83d3a-115">Application</span></span>                            | <span data-ttu-id="83d3a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d3a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83d3a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d3a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="83d3a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d3a-118">Request headers</span></span>

| <span data-ttu-id="83d3a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="83d3a-119">Name</span></span>          | <span data-ttu-id="83d3a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d3a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="83d3a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d3a-121">Authorization</span></span> | <span data-ttu-id="83d3a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83d3a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83d3a-124">Content-Type</span></span> | <span data-ttu-id="83d3a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d3a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83d3a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83d3a-127">Request body</span></span>

<span data-ttu-id="83d3a-128">No corpo da solicitação, fornece o identificador do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) (usando uma propriedade) que deve ser atribuído à `@odata.id` entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="83d3a-128">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="83d3a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d3a-129">Response</span></span>

<span data-ttu-id="83d3a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83d3a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83d3a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83d3a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83d3a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d3a-133">Request</span></span>

<span data-ttu-id="83d3a-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d3a-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="83d3a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="83d3a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="83d3a-136">C#</span><span class="sxs-lookup"><span data-stu-id="83d3a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83d3a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83d3a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83d3a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83d3a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83d3a-139">Java</span><span class="sxs-lookup"><span data-stu-id="83d3a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83d3a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d3a-140">Response</span></span>

<span data-ttu-id="83d3a-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83d3a-141">The following is an example of the response.</span></span>

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

