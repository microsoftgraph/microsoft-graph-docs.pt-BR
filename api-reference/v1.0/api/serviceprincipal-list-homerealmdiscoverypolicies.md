---
title: Lista atribuída homeRealmDiscoveryPolicies
description: Listar homeRealmDiscoveryPolicies atribuídos a uma entidade de serviço.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4e200e01ff36db17bbeb51c5d42da95c32f414c
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846212"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="4de26-103">Lista atribuída homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="4de26-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="4de26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4de26-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4de26-105">Lista os objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) que são atribuídos a um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="4de26-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4de26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4de26-106">Permissions</span></span>

<span data-ttu-id="4de26-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4de26-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4de26-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4de26-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4de26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4de26-109">Permission type</span></span>                        | <span data-ttu-id="4de26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4de26-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4de26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4de26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4de26-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4de26-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="4de26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4de26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4de26-114">Not supported.</span></span> |
| <span data-ttu-id="4de26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4de26-115">Application</span></span>                            | <span data-ttu-id="4de26-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4de26-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4de26-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4de26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4de26-118">Request headers</span></span>

| <span data-ttu-id="4de26-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4de26-119">Name</span></span>          | <span data-ttu-id="4de26-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4de26-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4de26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4de26-121">Authorization</span></span> | <span data-ttu-id="4de26-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4de26-122">Bearer {token}.</span></span> <span data-ttu-id="4de26-123">Required.</span><span class="sxs-lookup"><span data-stu-id="4de26-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4de26-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4de26-124">Request body</span></span>

<span data-ttu-id="4de26-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4de26-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4de26-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de26-126">Response</span></span>

<span data-ttu-id="4de26-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4de26-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4de26-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4de26-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4de26-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4de26-129">Request</span></span>

<span data-ttu-id="4de26-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4de26-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4de26-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4de26-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="4de26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4de26-132">Response</span></span>

<span data-ttu-id="4de26-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4de26-133">The following is an example of the response.</span></span>

> <span data-ttu-id="4de26-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="4de26-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4de26-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4de26-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
