---
title: Listar activityBasedTimeoutPolicies
description: Obtenha uma lista de objetos activityBasedTimeoutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30c2688d01e14a646f52930d3dd133f19c316d85
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227769"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="23934-103">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="23934-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="23934-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23934-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="23934-105">Obtenha uma lista de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="23934-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="23934-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23934-106">Permissions</span></span>

<span data-ttu-id="23934-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23934-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23934-109">Permission type</span></span>                        | <span data-ttu-id="23934-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23934-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23934-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23934-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23934-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="23934-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="23934-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23934-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23934-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23934-114">Not supported.</span></span> |
| <span data-ttu-id="23934-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23934-115">Application</span></span>                            | <span data-ttu-id="23934-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="23934-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="23934-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23934-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23934-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23934-118">Optional query parameters</span></span>

<span data-ttu-id="23934-119">Este método oferece suporte `$filter`ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23934-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="23934-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="23934-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="23934-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23934-121">Request headers</span></span>

| <span data-ttu-id="23934-122">Nome</span><span class="sxs-lookup"><span data-stu-id="23934-122">Name</span></span>      |<span data-ttu-id="23934-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="23934-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23934-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="23934-124">Authorization</span></span> | <span data-ttu-id="23934-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23934-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23934-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23934-127">Request body</span></span>

<span data-ttu-id="23934-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23934-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23934-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="23934-129">Response</span></span>

<span data-ttu-id="23934-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23934-130">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23934-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="23934-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23934-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23934-132">Request</span></span>

<span data-ttu-id="23934-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="23934-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
```

### <a name="response"></a><span data-ttu-id="23934-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="23934-134">Response</span></span>

<span data-ttu-id="23934-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23934-135">The following is an example of the response.</span></span>

> <span data-ttu-id="23934-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23934-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
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
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
