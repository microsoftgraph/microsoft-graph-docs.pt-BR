---
title: Obter homeRealmDiscoveryPolicy
description: Recupere as propriedades e os relacionamentos do objeto homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 665c489e45555ec4de2283ba50dd89af1def22f1
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234096"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="ab57f-103">Obter homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ab57f-103">Get homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab57f-104">Recupere as propriedades e os relacionamentos de um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab57f-104">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab57f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab57f-105">Permissions</span></span>

<span data-ttu-id="ab57f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab57f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab57f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab57f-108">Permission type</span></span>                        | <span data-ttu-id="ab57f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab57f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab57f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab57f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab57f-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab57f-111">Policy.Read.All</span></span> |
| <span data-ttu-id="ab57f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab57f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab57f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab57f-113">Not supported.</span></span> |
| <span data-ttu-id="ab57f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab57f-114">Application</span></span>                            | <span data-ttu-id="ab57f-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab57f-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab57f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab57f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab57f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab57f-117">Optional query parameters</span></span>

<span data-ttu-id="ab57f-118">Este método oferece suporte `$expand` aos `$select` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab57f-118">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab57f-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab57f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ab57f-120">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="ab57f-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab57f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab57f-121">Request headers</span></span>

| <span data-ttu-id="ab57f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ab57f-122">Name</span></span>      |<span data-ttu-id="ab57f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab57f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab57f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab57f-124">Authorization</span></span> | <span data-ttu-id="ab57f-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ab57f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab57f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab57f-126">Request body</span></span>

<span data-ttu-id="ab57f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab57f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab57f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab57f-128">Response</span></span>

<span data-ttu-id="ab57f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab57f-129">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab57f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab57f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab57f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab57f-131">Request</span></span>

<span data-ttu-id="ab57f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab57f-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="ab57f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab57f-133">Response</span></span>

<span data-ttu-id="ab57f-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab57f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="ab57f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab57f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->