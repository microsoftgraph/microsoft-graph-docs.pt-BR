---
title: Obter authenticationContextClassReference
description: Recupere as propriedades e as relações de um objeto authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 38d63cf4422332502d0595b3e00fed2f305c02c6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664521"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="e0855-103">Obter authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="e0855-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="e0855-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0855-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0855-105">Recupere as propriedades e as relações de um [objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="e0855-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0855-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0855-106">Permissions</span></span>

<span data-ttu-id="e0855-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0855-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0855-109">Permission type</span></span>                        | <span data-ttu-id="e0855-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0855-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="e0855-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0855-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0855-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e0855-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="e0855-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0855-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0855-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0855-114">Not supported.</span></span> |
|<span data-ttu-id="e0855-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0855-115">Application</span></span>                            | <span data-ttu-id="e0855-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e0855-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0855-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0855-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0855-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0855-118">Optional query parameters</span></span>

<span data-ttu-id="e0855-119">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0855-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0855-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0855-120">Request headers</span></span>

| <span data-ttu-id="e0855-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e0855-121">Name</span></span>      |<span data-ttu-id="e0855-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0855-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0855-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0855-123">Authorization</span></span> | <span data-ttu-id="e0855-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e0855-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0855-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0855-125">Request body</span></span>

<span data-ttu-id="e0855-126">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0855-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e0855-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e0855-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="e0855-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0855-128">Response</span></span>

<span data-ttu-id="e0855-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0855-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0855-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0855-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0855-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0855-131">Request</span></span>

<span data-ttu-id="e0855-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0855-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="e0855-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0855-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```
# <a name="c"></a>[<span data-ttu-id="e0855-134">C#</span><span class="sxs-lookup"><span data-stu-id="e0855-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0855-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0855-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0855-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0855-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0855-137">Java</span><span class="sxs-lookup"><span data-stu-id="e0855-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="e0855-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0855-138">Response</span></span>

<span data-ttu-id="e0855-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0855-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e0855-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0855-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
