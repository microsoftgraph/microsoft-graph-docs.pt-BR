---
title: Obter activityBasedTimeoutPolicy
description: Obter as propriedades de um objeto activityBasedTimeoutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d982e993ce9024fcadd810f1d20a804d41c5a04
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234065"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="5fab4-103">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="5fab4-103">Get activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fab4-104">Obter as propriedades de um objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5fab4-104">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fab4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fab4-105">Permissions</span></span>

<span data-ttu-id="5fab4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fab4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fab4-108">Permission type</span></span>                        | <span data-ttu-id="5fab4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fab4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5fab4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fab4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fab4-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fab4-111">Policy.Read.All</span></span> |
| <span data-ttu-id="5fab4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fab4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fab4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fab4-113">Not supported.</span></span> |
| <span data-ttu-id="5fab4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fab4-114">Application</span></span>                            | <span data-ttu-id="5fab4-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fab4-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fab4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fab4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fab4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fab4-117">Optional query parameters</span></span>

<span data-ttu-id="5fab4-118">Este método oferece suporte `$select` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5fab4-118">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5fab4-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5fab4-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fab4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fab4-120">Request headers</span></span>

| <span data-ttu-id="5fab4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5fab4-121">Name</span></span>      |<span data-ttu-id="5fab4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fab4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fab4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fab4-123">Authorization</span></span> | <span data-ttu-id="5fab4-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5fab4-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fab4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fab4-125">Request body</span></span>

<span data-ttu-id="5fab4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fab4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fab4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fab4-127">Response</span></span>

<span data-ttu-id="5fab4-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fab4-128">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fab4-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5fab4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fab4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fab4-130">Request</span></span>

<span data-ttu-id="5fab4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fab4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="5fab4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fab4-132">Response</span></span>

<span data-ttu-id="5fab4-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fab4-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5fab4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fab4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->