---
title: Listar tokenIssuancePolicy
description: Obtenha uma lista de objetos tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32242e6ad6f6285ba04df02688623a100224d818
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229672"
---
# <a name="list-tokenissuancepolicy"></a><span data-ttu-id="3d8a3-103">Listar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="3d8a3-103">List tokenIssuancePolicy</span></span>

<span data-ttu-id="3d8a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d8a3-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3d8a3-105">Obtenha uma lista de objetos [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3d8a3-105">Get a list of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d8a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d8a3-106">Permissions</span></span>

<span data-ttu-id="3d8a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d8a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d8a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d8a3-109">Permission type</span></span>                        | <span data-ttu-id="3d8a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d8a3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d8a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d8a3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d8a3-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d8a3-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="3d8a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d8a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d8a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-114">Not supported.</span></span> |
| <span data-ttu-id="3d8a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d8a3-115">Application</span></span>                            | <span data-ttu-id="3d8a3-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d8a3-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d8a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d8a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenIssuancePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d8a3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d8a3-118">Optional query parameters</span></span>

<span data-ttu-id="3d8a3-119">Este método oferece suporte `$expand`aos `$filter`parâmetros `$select`de consulta `$top` OData,, e OData, para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3d8a3-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3d8a3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="3d8a3-121">Ao usar `$expand`o, certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d8a3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d8a3-122">Request headers</span></span>

| <span data-ttu-id="3d8a3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3d8a3-123">Name</span></span>      |<span data-ttu-id="3d8a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d8a3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d8a3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d8a3-125">Authorization</span></span> | <span data-ttu-id="3d8a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d8a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d8a3-128">Request body</span></span>

<span data-ttu-id="3d8a3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d8a3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d8a3-130">Response</span></span>

<span data-ttu-id="3d8a3-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-131">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d8a3-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d8a3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d8a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d8a3-133">Request</span></span>

<span data-ttu-id="3d8a3-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "tokenIssuancePolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="3d8a3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d8a3-135">Response</span></span>

<span data-ttu-id="3d8a3-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-136">The following is an example of the response.</span></span>

> <span data-ttu-id="3d8a3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d8a3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
