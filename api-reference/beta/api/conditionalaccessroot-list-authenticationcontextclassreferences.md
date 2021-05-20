---
title: Listar authenticationContextClassReferences
description: Recupere uma lista de objetos authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c5ad949518d8371e18fc1ef10e680f618056b7f5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547308"
---
# <a name="list-authenticationcontextclassreferences"></a><span data-ttu-id="14af5-103">Listar authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="14af5-103">List authenticationContextClassReferences</span></span>

<span data-ttu-id="14af5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14af5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14af5-105">Recupere uma lista de [objetos authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="14af5-105">Retrieve a list of [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="14af5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="14af5-106">Permissions</span></span>

<span data-ttu-id="14af5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14af5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14af5-109">Permission type</span></span>                        | <span data-ttu-id="14af5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14af5-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="14af5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14af5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14af5-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="14af5-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="14af5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14af5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14af5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14af5-114">Not supported.</span></span> |
|<span data-ttu-id="14af5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14af5-115">Application</span></span>                            | <span data-ttu-id="14af5-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="14af5-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="14af5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14af5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14af5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14af5-118">Optional query parameters</span></span>

<span data-ttu-id="14af5-119">Este método dá suporte aos `$filter` `$select` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14af5-119">This method supports the `$filter` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="14af5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14af5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14af5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14af5-121">Request headers</span></span>

| <span data-ttu-id="14af5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="14af5-122">Name</span></span>      |<span data-ttu-id="14af5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="14af5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14af5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="14af5-124">Authorization</span></span> | <span data-ttu-id="14af5-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="14af5-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14af5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14af5-126">Request body</span></span>

<span data-ttu-id="14af5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14af5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14af5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="14af5-128">Response</span></span>

<span data-ttu-id="14af5-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14af5-129">If successful, this method returns a `200 OK` response code and a collection of [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14af5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14af5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14af5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14af5-131">Request</span></span>

<span data-ttu-id="14af5-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14af5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14af5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="14af5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
```



### <a name="response"></a><span data-ttu-id="14af5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="14af5-134">Response</span></span>

<span data-ttu-id="14af5-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14af5-135">The following is an example of the response.</span></span>

> <span data-ttu-id="14af5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14af5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#/conditionalAccess/authenticationContextClassReferences",
  "value": [
    {
      "id": "c1",
      "displayName": "Contoso trusted locations",
      "description": "Access is only allowed from trusted locations",
      "isAvailable": true
    }
  ]
}


```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List authenticationContextClassReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
