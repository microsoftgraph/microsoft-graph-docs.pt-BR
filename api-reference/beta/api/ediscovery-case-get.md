---
title: Obter caso
description: Recupere as propriedades e as relações de um objeto case.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d4785ba534ddbb334b87da5c0ddac3f8b32cb071
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776729"
---
# <a name="get-case"></a><span data-ttu-id="e0981-103">Obter caso</span><span class="sxs-lookup"><span data-stu-id="e0981-103">Get case</span></span>

<span data-ttu-id="e0981-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e0981-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0981-105">Recupere as propriedades e as relações de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="e0981-105">Retrieve the properties and relationships of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0981-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0981-106">Permissions</span></span>

<span data-ttu-id="e0981-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0981-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0981-109">Permission type</span></span>|<span data-ttu-id="e0981-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0981-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0981-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0981-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0981-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0981-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e0981-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0981-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0981-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0981-114">Not supported.</span></span>|
|<span data-ttu-id="e0981-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0981-115">Application</span></span>|<span data-ttu-id="e0981-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0981-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0981-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0981-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0981-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0981-118">Optional query parameters</span></span>

<span data-ttu-id="e0981-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0981-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e0981-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e0981-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0981-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0981-121">Request headers</span></span>

| <span data-ttu-id="e0981-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e0981-122">Name</span></span>      |<span data-ttu-id="e0981-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0981-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0981-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0981-124">Authorization</span></span> | <span data-ttu-id="e0981-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0981-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0981-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0981-127">Request body</span></span>

<span data-ttu-id="e0981-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0981-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0981-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0981-129">Response</span></span>

<span data-ttu-id="e0981-130">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0981-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0981-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0981-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0981-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0981-132">Request</span></span>

<span data-ttu-id="e0981-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0981-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0981-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0981-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```
# <a name="c"></a>[<span data-ttu-id="e0981-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0981-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0981-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0981-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0981-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0981-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0981-138">Java</span><span class="sxs-lookup"><span data-stu-id="e0981-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0981-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0981-139">Response</span></span>

<span data-ttu-id="e0981-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0981-140">The following is an example of the response.</span></span>

> <span data-ttu-id="e0981-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e0981-141">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
