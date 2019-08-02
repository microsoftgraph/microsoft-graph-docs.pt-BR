---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e os relacionamentos de um objeto featurerolloutpolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c36c8db23e0550ac1d68aea363ce7921d82a3a0
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062092"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="09e0a-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="09e0a-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e0a-104">Recupere as propriedades e os relacionamentos de um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="09e0a-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09e0a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09e0a-105">Permissions</span></span>

<span data-ttu-id="09e0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09e0a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09e0a-108">Permission type</span></span>                        | <span data-ttu-id="09e0a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09e0a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09e0a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09e0a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09e0a-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e0a-111">Policy.Read.All</span></span> |
| <span data-ttu-id="09e0a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09e0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09e0a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09e0a-113">Not supported.</span></span> |
| <span data-ttu-id="09e0a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09e0a-114">Application</span></span>                            | <span data-ttu-id="09e0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09e0a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09e0a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09e0a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09e0a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09e0a-117">Optional query parameters</span></span>

<span data-ttu-id="09e0a-118">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09e0a-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="09e0a-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="09e0a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="09e0a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09e0a-120">Request headers</span></span>

| <span data-ttu-id="09e0a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="09e0a-121">Name</span></span>      |<span data-ttu-id="09e0a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="09e0a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09e0a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e0a-123">Authorization</span></span> | <span data-ttu-id="09e0a-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="09e0a-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09e0a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09e0a-125">Request body</span></span>

<span data-ttu-id="09e0a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09e0a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09e0a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="09e0a-127">Response</span></span>

<span data-ttu-id="09e0a-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09e0a-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09e0a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09e0a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09e0a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09e0a-130">Request</span></span>

<span data-ttu-id="09e0a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09e0a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="09e0a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="09e0a-132">Response</span></span>

<span data-ttu-id="09e0a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09e0a-133">The following is an example of the response.</span></span>

> <span data-ttu-id="09e0a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09e0a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="09e0a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09e0a-136">Request</span></span>

<span data-ttu-id="09e0a-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09e0a-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

### <a name="response"></a><span data-ttu-id="09e0a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="09e0a-138">Response</span></span>

<span data-ttu-id="09e0a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09e0a-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="09e0a-140">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09e0a-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09e0a-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09e0a-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
