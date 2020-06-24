---
title: Obter claimsMappingPolicy
description: Recupere as propriedades e os relacionamentos de um objeto claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 10213a3112ab3b05f1e5b3dcfa4fe497dfadfc36
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846198"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="598ab-103">Obter claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="598ab-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="598ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="598ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="598ab-105">Recupere as propriedades e os relacionamentos de um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="598ab-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="598ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="598ab-106">Permissions</span></span>

<span data-ttu-id="598ab-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="598ab-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="598ab-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="598ab-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="598ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="598ab-109">Permission type</span></span>                        | <span data-ttu-id="598ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="598ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="598ab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="598ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="598ab-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="598ab-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="598ab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="598ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="598ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="598ab-114">Not supported.</span></span> |
| <span data-ttu-id="598ab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="598ab-115">Application</span></span>                            | <span data-ttu-id="598ab-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="598ab-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="598ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="598ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="598ab-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="598ab-118">Optional query parameters</span></span>

<span data-ttu-id="598ab-119">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="598ab-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="598ab-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="598ab-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="598ab-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="598ab-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="598ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="598ab-122">Request headers</span></span>

| <span data-ttu-id="598ab-123">Nome</span><span class="sxs-lookup"><span data-stu-id="598ab-123">Name</span></span>      |<span data-ttu-id="598ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="598ab-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="598ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="598ab-125">Authorization</span></span> | <span data-ttu-id="598ab-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="598ab-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="598ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="598ab-127">Request body</span></span>

<span data-ttu-id="598ab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="598ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="598ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="598ab-129">Response</span></span>

<span data-ttu-id="598ab-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="598ab-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="598ab-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="598ab-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="598ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="598ab-132">Request</span></span>

<span data-ttu-id="598ab-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="598ab-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="598ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="598ab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="598ab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="598ab-135">Response</span></span>

<span data-ttu-id="598ab-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="598ab-136">The following is an example of the response.</span></span>

> <span data-ttu-id="598ab-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="598ab-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="598ab-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="598ab-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
