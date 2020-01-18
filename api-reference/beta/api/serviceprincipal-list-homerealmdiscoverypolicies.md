---
title: Lista atribuída homeRealmDiscoveryPolicies
description: Listar homeRealmDiscoveryPolicies atribuídos a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce4d82ae36a7451c44e266f02953b7e7b7705090
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234100"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="0c49c-103">Lista atribuída homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="0c49c-103">List assigned homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c49c-104">Lista os objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) que são atribuídos a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0c49c-104">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c49c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c49c-105">Permissions</span></span>

<span data-ttu-id="0c49c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c49c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c49c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c49c-108">Permission type</span></span>                        | <span data-ttu-id="0c49c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c49c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0c49c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c49c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c49c-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0c49c-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0c49c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c49c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c49c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c49c-113">Not supported.</span></span> |
| <span data-ttu-id="0c49c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c49c-114">Application</span></span>                            | <span data-ttu-id="0c49c-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0c49c-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c49c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c49c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0c49c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c49c-117">Request headers</span></span>

| <span data-ttu-id="0c49c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0c49c-118">Name</span></span>          | <span data-ttu-id="0c49c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c49c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0c49c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c49c-120">Authorization</span></span> | <span data-ttu-id="0c49c-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0c49c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c49c-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c49c-122">Request body</span></span>

<span data-ttu-id="0c49c-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c49c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c49c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c49c-124">Response</span></span>

<span data-ttu-id="0c49c-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c49c-125">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c49c-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c49c-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c49c-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c49c-127">Request</span></span>

<span data-ttu-id="0c49c-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c49c-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="0c49c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c49c-129">Response</span></span>

<span data-ttu-id="0c49c-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c49c-130">The following is an example of the response.</span></span>

> <span data-ttu-id="0c49c-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c49c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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