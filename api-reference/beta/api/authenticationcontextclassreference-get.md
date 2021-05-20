---
title: Obter authenticationContextClassReference
description: Recupere as propriedades e as relações de um objeto authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3ca46a2dfff70ed32bc2e960b4f16cdca9ab7da8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547294"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="b1efc-103">Obter authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="b1efc-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="b1efc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1efc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1efc-105">Recupere as propriedades e as relações de um [objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="b1efc-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1efc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1efc-106">Permissions</span></span>

<span data-ttu-id="b1efc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1efc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1efc-109">Permission type</span></span>                        | <span data-ttu-id="b1efc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1efc-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="b1efc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1efc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1efc-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b1efc-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="b1efc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1efc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1efc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1efc-114">Not supported.</span></span> |
|<span data-ttu-id="b1efc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1efc-115">Application</span></span>                            | <span data-ttu-id="b1efc-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b1efc-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1efc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1efc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1efc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1efc-118">Optional query parameters</span></span>

<span data-ttu-id="b1efc-119">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1efc-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1efc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1efc-120">Request headers</span></span>

| <span data-ttu-id="b1efc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b1efc-121">Name</span></span>      |<span data-ttu-id="b1efc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1efc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b1efc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1efc-123">Authorization</span></span> | <span data-ttu-id="b1efc-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b1efc-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1efc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1efc-125">Request body</span></span>

<span data-ttu-id="b1efc-126">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1efc-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="b1efc-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b1efc-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="b1efc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1efc-128">Response</span></span>

<span data-ttu-id="b1efc-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1efc-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1efc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b1efc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1efc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1efc-131">Request</span></span>

<span data-ttu-id="b1efc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1efc-132">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```



### <a name="response"></a><span data-ttu-id="b1efc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1efc-133">Response</span></span>

<span data-ttu-id="b1efc-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1efc-134">The following is an example of the response.</span></span>

> <span data-ttu-id="b1efc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1efc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReferences/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": false
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
