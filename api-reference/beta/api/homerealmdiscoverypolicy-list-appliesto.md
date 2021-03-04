---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cf4d398a065139f752d604d552a3c73f71f495b9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435676"
---
# <a name="list-appliesto"></a><span data-ttu-id="da149-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="da149-103">List appliesTo</span></span>

<span data-ttu-id="da149-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da149-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da149-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="da149-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="da149-106">O homeRealmDiscoveryPolicy só pode ser aplicado aos [recursos servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="da149-106">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="da149-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="da149-107">Permissions</span></span>

<span data-ttu-id="da149-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da149-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da149-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da149-110">Permission type</span></span>                        | <span data-ttu-id="da149-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da149-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da149-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da149-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="da149-113">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da149-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="da149-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da149-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da149-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da149-115">Not supported.</span></span> |
| <span data-ttu-id="da149-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da149-116">Application</span></span>                            | <span data-ttu-id="da149-117">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da149-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da149-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da149-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da149-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da149-119">Optional query parameters</span></span>

<span data-ttu-id="da149-120">Este método dá suporte aos `$select` `$top` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da149-120">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="da149-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da149-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da149-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da149-122">Request headers</span></span>

| <span data-ttu-id="da149-123">Nome</span><span class="sxs-lookup"><span data-stu-id="da149-123">Name</span></span>      |<span data-ttu-id="da149-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="da149-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da149-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da149-125">Authorization</span></span> | <span data-ttu-id="da149-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="da149-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="da149-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da149-127">Request body</span></span>

<span data-ttu-id="da149-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da149-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da149-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="da149-129">Response</span></span>

<span data-ttu-id="da149-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da149-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da149-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da149-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da149-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da149-132">Request</span></span>

<span data-ttu-id="da149-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da149-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="da149-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="da149-134">Response</span></span>

<span data-ttu-id="da149-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da149-135">The following is an example of the response.</span></span>

> <span data-ttu-id="da149-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da149-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

