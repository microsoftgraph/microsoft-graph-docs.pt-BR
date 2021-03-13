---
title: Listar operações
description: Obter a lista caseOperations de um objeto case.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ee95efa24aa1f7a3c0254e3da2e22cc43e3568c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776680"
---
# <a name="list-operations"></a><span data-ttu-id="5c837-103">Listar operações</span><span class="sxs-lookup"><span data-stu-id="5c837-103">List operations</span></span>

<span data-ttu-id="5c837-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5c837-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c837-105">Obter a lista [de caseOperations](../resources/ediscovery-caseoperation.md) de um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="5c837-105">Get the list of [caseOperations](../resources/ediscovery-caseoperation.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c837-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c837-106">Permissions</span></span>

<span data-ttu-id="5c837-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c837-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c837-109">Permission type</span></span>|<span data-ttu-id="5c837-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c837-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c837-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c837-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c837-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c837-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5c837-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c837-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c837-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c837-114">Not supported.</span></span>|
|<span data-ttu-id="5c837-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c837-115">Application</span></span>|<span data-ttu-id="5c837-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c837-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c837-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c837-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c837-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c837-118">Optional query parameters</span></span>

<span data-ttu-id="5c837-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c837-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c837-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c837-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c837-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c837-121">Request headers</span></span>

|<span data-ttu-id="5c837-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5c837-122">Name</span></span>|<span data-ttu-id="5c837-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c837-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c837-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c837-124">Authorization</span></span>|<span data-ttu-id="5c837-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c837-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c837-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c837-127">Request body</span></span>
<span data-ttu-id="5c837-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c837-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c837-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c837-129">Response</span></span>

<span data-ttu-id="5c837-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c837-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c837-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c837-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c837-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c837-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5c837-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c837-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_caseoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations
```
# <a name="c"></a>[<span data-ttu-id="5c837-134">C#</span><span class="sxs-lookup"><span data-stu-id="5c837-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-caseoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c837-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c837-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-caseoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c837-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c837-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-caseoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c837-137">Java</span><span class="sxs-lookup"><span data-stu-id="5c837-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-caseoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c837-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c837-138">Response</span></span>

<span data-ttu-id="5c837-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c837-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.caseOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
      "id": "41362b70-2b70-4136-702b-3641702b3641",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
