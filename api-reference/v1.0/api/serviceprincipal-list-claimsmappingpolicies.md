---
title: Lista atribuída claimsMappingPolicies
description: Listar claimsMappingPolicies atribuídos a uma entidade de serviço.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c5310d84dae2d2d0a32b8511a1c02eccb977fa5
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846213"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="69940-103">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="69940-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="69940-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69940-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="69940-105">Lista os objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) que são atribuídos a um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="69940-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69940-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69940-106">Permissions</span></span>

<span data-ttu-id="69940-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="69940-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="69940-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69940-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69940-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69940-109">Permission type</span></span>                        | <span data-ttu-id="69940-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69940-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69940-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69940-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="69940-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="69940-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="69940-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69940-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69940-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69940-114">Not supported.</span></span> |
| <span data-ttu-id="69940-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69940-115">Application</span></span>                            | <span data-ttu-id="69940-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="69940-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69940-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69940-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="69940-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69940-118">Request headers</span></span>

| <span data-ttu-id="69940-119">Nome</span><span class="sxs-lookup"><span data-stu-id="69940-119">Name</span></span>          | <span data-ttu-id="69940-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69940-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="69940-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69940-121">Authorization</span></span> | <span data-ttu-id="69940-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="69940-122">Bearer {token}.</span></span> <span data-ttu-id="69940-123">Required.</span><span class="sxs-lookup"><span data-stu-id="69940-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69940-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69940-124">Request body</span></span>

<span data-ttu-id="69940-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69940-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69940-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="69940-126">Response</span></span>

<span data-ttu-id="69940-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69940-127">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="69940-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69940-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69940-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69940-129">Request</span></span>

<span data-ttu-id="69940-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69940-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="69940-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="69940-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies
```

### <a name="response"></a><span data-ttu-id="69940-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="69940-132">Response</span></span>

<span data-ttu-id="69940-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69940-133">The following is an example of the response.</span></span>

> <span data-ttu-id="69940-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="69940-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="69940-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="69940-135">All the properties will be returned from an actual call.</span></span>

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
