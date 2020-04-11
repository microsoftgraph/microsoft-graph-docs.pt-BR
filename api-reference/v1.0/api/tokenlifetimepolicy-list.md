---
title: Listar tokenLifetimePolicies
description: Obtenha uma lista de objetos tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8ef186128a428b9bc999a14fc61a588a4eb7859
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229539"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="06ccb-103">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="06ccb-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="06ccb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06ccb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="06ccb-105">Obtenha uma lista de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="06ccb-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="06ccb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06ccb-106">Permissions</span></span>

<span data-ttu-id="06ccb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06ccb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06ccb-109">Permission type</span></span>                        | <span data-ttu-id="06ccb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06ccb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06ccb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06ccb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06ccb-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="06ccb-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="06ccb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06ccb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06ccb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ccb-114">Not supported.</span></span> |
| <span data-ttu-id="06ccb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ccb-115">Application</span></span>                            | <span data-ttu-id="06ccb-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="06ccb-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="06ccb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06ccb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06ccb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06ccb-118">Optional query parameters</span></span>

<span data-ttu-id="06ccb-119">Este método oferece suporte `$expand`a `$filter`, `$select` e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06ccb-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="06ccb-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="06ccb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="06ccb-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="06ccb-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06ccb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06ccb-122">Request headers</span></span>

| <span data-ttu-id="06ccb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="06ccb-123">Name</span></span>      |<span data-ttu-id="06ccb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="06ccb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06ccb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="06ccb-125">Authorization</span></span> | <span data-ttu-id="06ccb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06ccb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06ccb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06ccb-128">Request body</span></span>

<span data-ttu-id="06ccb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06ccb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06ccb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ccb-130">Response</span></span>

<span data-ttu-id="06ccb-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06ccb-131">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06ccb-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06ccb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06ccb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06ccb-133">Request</span></span>

<span data-ttu-id="06ccb-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06ccb-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="06ccb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ccb-135">Response</span></span>

<span data-ttu-id="06ccb-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06ccb-136">The following is an example of the response.</span></span>

> <span data-ttu-id="06ccb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06ccb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
