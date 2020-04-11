---
title: Listar homeRealmDiscoveryPolicies
description: Obtenha uma lista de objetos homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12c2026e78b0d4915640e967b32132b9cefa4126
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227752"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="acdff-103">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="acdff-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="acdff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acdff-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="acdff-105">Obtenha uma lista de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="acdff-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="acdff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="acdff-106">Permissions</span></span>

<span data-ttu-id="acdff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acdff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acdff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acdff-109">Permission type</span></span>                        | <span data-ttu-id="acdff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acdff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="acdff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acdff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="acdff-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="acdff-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="acdff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acdff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acdff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acdff-114">Not supported.</span></span> |
| <span data-ttu-id="acdff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acdff-115">Application</span></span>                            | <span data-ttu-id="acdff-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="acdff-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="acdff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acdff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acdff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="acdff-118">Optional query parameters</span></span>

<span data-ttu-id="acdff-119">Este método oferece suporte `$expand`aos `$filter`parâmetros `$select`de consulta `$top` OData,, e OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="acdff-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="acdff-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="acdff-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="acdff-121">Ao usar `$expand`o, certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="acdff-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acdff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acdff-122">Request headers</span></span>

| <span data-ttu-id="acdff-123">Nome</span><span class="sxs-lookup"><span data-stu-id="acdff-123">Name</span></span>      |<span data-ttu-id="acdff-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="acdff-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acdff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="acdff-125">Authorization</span></span> | <span data-ttu-id="acdff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acdff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acdff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acdff-128">Request body</span></span>

<span data-ttu-id="acdff-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acdff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acdff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="acdff-130">Response</span></span>

<span data-ttu-id="acdff-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acdff-131">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="acdff-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="acdff-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="acdff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acdff-133">Request</span></span>

<span data-ttu-id="acdff-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="acdff-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="acdff-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="acdff-135">Response</span></span>

<span data-ttu-id="acdff-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="acdff-136">The following is an example of the response.</span></span>

> <span data-ttu-id="acdff-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acdff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List homeRealmDiscoveryPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
