---
title: Listar featureRolloutPolicies
description: Recupere uma lista de objetos featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0b6d28265d3f64a278e624d7fe17ded39072e772
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952188"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="b14b4-103">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="b14b4-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="b14b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b14b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b14b4-105">Recupere uma lista de [objetos featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b14b4-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b14b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b14b4-106">Permissions</span></span>

<span data-ttu-id="b14b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b14b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b14b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b14b4-109">Permission type</span></span>                        | <span data-ttu-id="b14b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b14b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b14b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b14b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b14b4-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b14b4-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b14b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b14b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b14b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b14b4-114">Not supported.</span></span> |
| <span data-ttu-id="b14b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b14b4-115">Application</span></span>                            | <span data-ttu-id="b14b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b14b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b14b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b14b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b14b4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b14b4-118">Optional query parameters</span></span>

<span data-ttu-id="b14b4-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta: `$count` , , , , , , `$expand` `$filter` `$orderby` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b14b4-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="b14b4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b14b4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b14b4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b14b4-121">Request headers</span></span>

| <span data-ttu-id="b14b4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b14b4-122">Name</span></span>      |<span data-ttu-id="b14b4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b14b4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b14b4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b14b4-124">Authorization</span></span> | <span data-ttu-id="b14b4-125">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="b14b4-125">Bearer {token}.</span></span> <span data-ttu-id="b14b4-126">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b14b4-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="b14b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b14b4-127">Request body</span></span>

<span data-ttu-id="b14b4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b14b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b14b4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b14b4-129">Response</span></span>

<span data-ttu-id="b14b4-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b14b4-130">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b14b4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b14b4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b14b4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b14b4-132">Request</span></span>

<span data-ttu-id="b14b4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b14b4-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies
```

### <a name="response"></a><span data-ttu-id="b14b4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b14b4-134">Response</span></span>

<span data-ttu-id="b14b4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b14b4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b14b4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b14b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


