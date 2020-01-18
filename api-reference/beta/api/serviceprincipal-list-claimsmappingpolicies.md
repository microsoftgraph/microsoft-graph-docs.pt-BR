---
title: Lista atribuída claimsMappingPolicies
description: Listar claimsMappingPolicies atribuídos a um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0630a82e1cc69dbb6a760aaa6a6fb52a79e06aee
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234098"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="f7537-103">Lista atribuída claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="f7537-103">List assigned claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7537-104">Lista os objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) que são atribuídos a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f7537-104">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7537-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7537-105">Permissions</span></span>

<span data-ttu-id="f7537-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7537-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7537-108">Permission type</span></span>                        | <span data-ttu-id="f7537-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7537-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7537-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7537-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7537-111">Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7537-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="f7537-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7537-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7537-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7537-113">Not supported.</span></span> |
| <span data-ttu-id="f7537-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7537-114">Application</span></span>                            | <span data-ttu-id="f7537-115">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7537-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7537-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7537-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f7537-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7537-117">Request headers</span></span>

| <span data-ttu-id="f7537-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f7537-118">Name</span></span>          | <span data-ttu-id="f7537-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7537-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7537-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7537-120">Authorization</span></span> | <span data-ttu-id="f7537-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f7537-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7537-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7537-122">Request body</span></span>

<span data-ttu-id="f7537-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7537-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7537-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7537-124">Response</span></span>

<span data-ttu-id="f7537-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsMappingPolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7537-125">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7537-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7537-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7537-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7537-127">Request</span></span>

<span data-ttu-id="f7537-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7537-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```

### <a name="response"></a><span data-ttu-id="f7537-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7537-129">Response</span></span>

<span data-ttu-id="f7537-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7537-130">The following is an example of the response.</span></span>

> <span data-ttu-id="f7537-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7537-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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