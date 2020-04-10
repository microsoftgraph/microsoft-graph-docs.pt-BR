---
title: Lista atribuída claimsMappingPolicies
description: Listar claimsMappingPolicies atribuídos a um servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83bad7c305506814bdd931dcf29a4a3513625fd3
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219085"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="69344-103">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="69344-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="69344-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69344-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69344-105">Lista os objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) que são atribuídos a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="69344-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69344-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69344-106">Permissions</span></span>

<span data-ttu-id="69344-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69344-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69344-109">Permission type</span></span>                        | <span data-ttu-id="69344-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69344-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69344-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69344-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="69344-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="69344-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="69344-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69344-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69344-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69344-114">Not supported.</span></span> |
| <span data-ttu-id="69344-115">Application</span><span class="sxs-lookup"><span data-stu-id="69344-115">Application</span></span>                            | <span data-ttu-id="69344-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="69344-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69344-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69344-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="69344-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69344-118">Request headers</span></span>

| <span data-ttu-id="69344-119">Nome</span><span class="sxs-lookup"><span data-stu-id="69344-119">Name</span></span>          | <span data-ttu-id="69344-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69344-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="69344-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69344-121">Authorization</span></span> | <span data-ttu-id="69344-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="69344-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="69344-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69344-123">Request body</span></span>

<span data-ttu-id="69344-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69344-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69344-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="69344-125">Response</span></span>

<span data-ttu-id="69344-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsMappingPolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69344-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69344-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69344-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69344-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69344-128">Request</span></span>

<span data-ttu-id="69344-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69344-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69344-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="69344-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="69344-131">C#</span><span class="sxs-lookup"><span data-stu-id="69344-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69344-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69344-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69344-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69344-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69344-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="69344-134">Response</span></span>

<span data-ttu-id="69344-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69344-135">The following is an example of the response.</span></span>

> <span data-ttu-id="69344-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69344-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
