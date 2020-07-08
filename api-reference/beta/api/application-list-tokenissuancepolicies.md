---
title: Lista atribuída tokenIssuancePolicies
description: Listar tokenIssuancePolicies atribuídos a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99e6811d3462afd64548063685e20225459d0f3a
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081268"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="adda5-103">Lista atribuída tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="adda5-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="adda5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adda5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adda5-105">Lista os objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="adda5-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="adda5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="adda5-106">Permissions</span></span>

<span data-ttu-id="adda5-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="adda5-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="adda5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adda5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adda5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adda5-109">Permission type</span></span>                        | <span data-ttu-id="adda5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adda5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adda5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adda5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adda5-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="adda5-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="adda5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adda5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adda5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adda5-114">Not supported.</span></span> |
| <span data-ttu-id="adda5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adda5-115">Application</span></span>                            | <span data-ttu-id="adda5-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="adda5-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adda5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adda5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="adda5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adda5-118">Request headers</span></span>

| <span data-ttu-id="adda5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="adda5-119">Name</span></span>          | <span data-ttu-id="adda5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="adda5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="adda5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="adda5-121">Authorization</span></span> | <span data-ttu-id="adda5-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="adda5-122">Bearer {token}.</span></span> <span data-ttu-id="adda5-123">Required.</span><span class="sxs-lookup"><span data-stu-id="adda5-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adda5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adda5-124">Request body</span></span>

<span data-ttu-id="adda5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adda5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adda5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="adda5-126">Response</span></span>

<span data-ttu-id="adda5-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adda5-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adda5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="adda5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adda5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adda5-129">Request</span></span>

<span data-ttu-id="adda5-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="adda5-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="adda5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="adda5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="adda5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="adda5-132">Response</span></span>

<span data-ttu-id="adda5-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="adda5-133">The following is an example of the response.</span></span>

> <span data-ttu-id="adda5-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="adda5-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="adda5-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="adda5-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
