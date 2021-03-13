---
title: Listar printServiceEndpoints
description: Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 16e32eec5580990c3ea80f4f6e596188d08103a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777044"
---
# <a name="list-endpoints"></a><span data-ttu-id="4c009-103">Listar pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="4c009-103">List endpoints</span></span>
<span data-ttu-id="4c009-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4c009-105">Recupere uma lista de pontos de extremidade expostos por um serviço de impressão.</span><span class="sxs-lookup"><span data-stu-id="4c009-105">Retrieve a list of endpoints exposed by a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c009-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4c009-106">Permissions</span></span>
<span data-ttu-id="4c009-107">Uma das permissões **de** Impressão Universal delegada [é](/graph/permissions-reference#universal-print-permissions) necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4c009-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="4c009-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c009-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services/{printServiceId}/endpoints
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c009-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c009-109">Optional query parameters</span></span>
<span data-ttu-id="4c009-110">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c009-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c009-111">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c009-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c009-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c009-112">Request headers</span></span>
|<span data-ttu-id="4c009-113">Nome</span><span class="sxs-lookup"><span data-stu-id="4c009-113">Name</span></span>|<span data-ttu-id="4c009-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c009-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4c009-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c009-115">Authorization</span></span>|<span data-ttu-id="4c009-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c009-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c009-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c009-118">Request body</span></span>
<span data-ttu-id="4c009-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c009-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c009-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c009-120">Response</span></span>

<span data-ttu-id="4c009-121">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printServiceEndpoint](../resources/printserviceendpoint.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c009-121">If successful, this method returns a `200 OK` response code and a collection of [printServiceEndpoint](../resources/printserviceendpoint.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c009-122">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c009-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c009-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c009-123">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4c009-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c009-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printserviceendpoint"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}/endpoints
```
# <a name="c"></a>[<span data-ttu-id="4c009-125">C#</span><span class="sxs-lookup"><span data-stu-id="4c009-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c009-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c009-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c009-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c009-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c009-128">Java</span><span class="sxs-lookup"><span data-stu-id="4c009-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printserviceendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4c009-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c009-129">Response</span></span>
<span data-ttu-id="4c009-130">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c009-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printServiceEndpoint)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "value": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

