---
title: Lista atribuída claimsMappingPolicies
description: Listar claimsMappingPolicies atribuídos a um servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c92dae5381b1c9b2364994e8859185b054485862
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044603"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="d82ef-103">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="d82ef-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="d82ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d82ef-105">Lista os objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) que são atribuídos a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="d82ef-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d82ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d82ef-106">Permissions</span></span>

<span data-ttu-id="d82ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d82ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d82ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d82ef-109">Permission type</span></span>                        | <span data-ttu-id="d82ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d82ef-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d82ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d82ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d82ef-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d82ef-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="d82ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d82ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d82ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d82ef-114">Not supported.</span></span> |
| <span data-ttu-id="d82ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d82ef-115">Application</span></span>                            | <span data-ttu-id="d82ef-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d82ef-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d82ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d82ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d82ef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ef-118">Request headers</span></span>

| <span data-ttu-id="d82ef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d82ef-119">Name</span></span>          | <span data-ttu-id="d82ef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d82ef-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d82ef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d82ef-121">Authorization</span></span> | <span data-ttu-id="d82ef-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d82ef-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d82ef-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ef-123">Request body</span></span>

<span data-ttu-id="d82ef-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d82ef-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d82ef-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82ef-125">Response</span></span>

<span data-ttu-id="d82ef-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsMappingPolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82ef-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d82ef-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d82ef-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d82ef-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ef-128">Request</span></span>

<span data-ttu-id="d82ef-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82ef-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d82ef-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d82ef-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="d82ef-131">C#</span><span class="sxs-lookup"><span data-stu-id="d82ef-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d82ef-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d82ef-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d82ef-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d82ef-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d82ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82ef-134">Response</span></span>

<span data-ttu-id="d82ef-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d82ef-135">The following is an example of the response.</span></span>

> <span data-ttu-id="d82ef-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d82ef-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


