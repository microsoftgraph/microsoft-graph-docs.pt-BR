---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 369a852668e56794311bafb2c53b0e692ad3efd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446533"
---
# <a name="list-appliesto"></a><span data-ttu-id="ce4bd-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="ce4bd-103">List appliesTo</span></span>

<span data-ttu-id="ce4bd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce4bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce4bd-105">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="ce4bd-106">O homeRealmDiscoveryPolicy só pode ser aplicado aos recursos do [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ce4bd-106">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce4bd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce4bd-107">Permissions</span></span>

<span data-ttu-id="ce4bd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce4bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce4bd-110">Permission type</span></span>                        | <span data-ttu-id="ce4bd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce4bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce4bd-113">Policy. Read. All e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ce4bd-113">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ce4bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce4bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce4bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-115">Not supported.</span></span> |
| <span data-ttu-id="ce4bd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce4bd-116">Application</span></span>                            | <span data-ttu-id="ce4bd-117">Policy. Read. All e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ce4bd-117">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce4bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce4bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce4bd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce4bd-119">Optional query parameters</span></span>

<span data-ttu-id="ce4bd-120">Este método oferece suporte `$select` aos `$top` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-120">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce4bd-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ce4bd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce4bd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-122">Request headers</span></span>

| <span data-ttu-id="ce4bd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ce4bd-123">Name</span></span>      |<span data-ttu-id="ce4bd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce4bd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce4bd-125">Authorization</span></span> | <span data-ttu-id="ce4bd-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ce4bd-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce4bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-127">Request body</span></span>

<span data-ttu-id="ce4bd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce4bd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bd-129">Response</span></span>

<span data-ttu-id="ce4bd-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce4bd-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce4bd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce4bd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bd-132">Request</span></span>

<span data-ttu-id="ce4bd-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="ce4bd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bd-134">Response</span></span>

<span data-ttu-id="ce4bd-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ce4bd-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce4bd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->