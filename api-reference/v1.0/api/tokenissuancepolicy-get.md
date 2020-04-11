---
title: Obter tokenIssuancePolicy
description: Recupere as propriedades e os relacionamentos do objeto tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c04068e65757faeccfcee4f75574b8494fd6fe2
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229686"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="41a1e-103">Obter tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="41a1e-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="41a1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41a1e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="41a1e-105">Recupere as propriedades e os relacionamentos de um objeto [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="41a1e-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41a1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41a1e-106">Permissions</span></span>

<span data-ttu-id="41a1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41a1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41a1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41a1e-109">Permission type</span></span>                        | <span data-ttu-id="41a1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41a1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41a1e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41a1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41a1e-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="41a1e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="41a1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41a1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41a1e-114">Not supported.</span></span> |
| <span data-ttu-id="41a1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41a1e-115">Application</span></span>                            | <span data-ttu-id="41a1e-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="41a1e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="41a1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41a1e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41a1e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41a1e-118">Optional query parameters</span></span>

<span data-ttu-id="41a1e-119">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41a1e-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="41a1e-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="41a1e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="41a1e-121">Ao usar `$expand`o, certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="41a1e-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41a1e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41a1e-122">Request headers</span></span>

| <span data-ttu-id="41a1e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="41a1e-123">Name</span></span>      |<span data-ttu-id="41a1e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="41a1e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41a1e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="41a1e-125">Authorization</span></span> | <span data-ttu-id="41a1e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41a1e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41a1e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41a1e-128">Request body</span></span>

<span data-ttu-id="41a1e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41a1e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41a1e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41a1e-130">Response</span></span>

<span data-ttu-id="41a1e-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41a1e-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41a1e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41a1e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41a1e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41a1e-133">Request</span></span>

<span data-ttu-id="41a1e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41a1e-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancepolicies/{id}
```

### <a name="response"></a><span data-ttu-id="41a1e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="41a1e-135">Response</span></span>

<span data-ttu-id="41a1e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41a1e-136">The following is an example of the response.</span></span>

> <span data-ttu-id="41a1e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41a1e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
