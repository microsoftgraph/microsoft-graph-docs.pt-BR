---
title: Listar monthlyPrintUsageByPrinter
description: Recupere uma lista de resumos de uso de impressão mensal, agrupados por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 19eff0d2fd6de0aad79a63cde61706db0c58f125
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781202"
---
# <a name="list-monthlyprintusagebyprinter"></a><span data-ttu-id="4bec3-103">Listar monthlyPrintUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="4bec3-103">List monthlyPrintUsageByPrinter</span></span>

<span data-ttu-id="4bec3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bec3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bec3-105">Recupere uma lista de resumos de uso de impressão mensal, agrupados por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="4bec3-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bec3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bec3-106">Permissions</span></span>
<span data-ttu-id="4bec3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4bec3-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="4bec3-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4bec3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bec3-110">Permission type</span></span> | <span data-ttu-id="4bec3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bec3-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4bec3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bec3-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4bec3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bec3-113">Reports.Read.All</span></span> |
|<span data-ttu-id="4bec3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bec3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bec3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bec3-115">Not Supported.</span></span>|
|<span data-ttu-id="4bec3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bec3-116">Application</span></span>|<span data-ttu-id="4bec3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bec3-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bec3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bec3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageByPrinter
GET /print/reports/monthlyPrintUsageByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="4bec3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bec3-119">Request headers</span></span>
| <span data-ttu-id="4bec3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4bec3-120">Name</span></span>      |<span data-ttu-id="4bec3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bec3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4bec3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bec3-122">Authorization</span></span> | <span data-ttu-id="4bec3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bec3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bec3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bec3-125">Request body</span></span>
<span data-ttu-id="4bec3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bec3-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4bec3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bec3-127">Response</span></span>
<span data-ttu-id="4bec3-128">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageByPrinter](../resources/printUsageByPrinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bec3-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageByPrinter](../resources/printUsageByPrinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bec3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bec3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bec3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bec3-130">Request</span></span>
<span data-ttu-id="4bec3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bec3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bec3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bec3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_5"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageByPrinter
```
# <a name="c"></a>[<span data-ttu-id="4bec3-133">C#</span><span class="sxs-lookup"><span data-stu-id="4bec3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bec3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bec3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bec3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bec3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bec3-136">Java</span><span class="sxs-lookup"><span data-stu-id="4bec3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4bec3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bec3-137">Response</span></span>
<span data-ttu-id="4bec3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bec3-138">The following is an example of the response.</span></span>
><span data-ttu-id="4bec3-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4bec3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "2020-02-04T00:00:00.0000000Z",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List monthlyPrintUsageByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


