---
title: Listar monthlyPrintUsageSummariesByPrinter
description: Recupere uma lista de resumos de uso de impressão mensal, agrupadas por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4e79046e023128546d438e7afae29882f98a1346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017273"
---
# <a name="list-monthlyprintusagesummariesbyprinter"></a><span data-ttu-id="3b1f6-103">Listar monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="3b1f6-103">List monthlyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="3b1f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1f6-105">Recupere uma lista de resumos de uso de impressão mensal, agrupadas por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="3b1f6-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b1f6-106">Permissions</span></span>
<span data-ttu-id="3b1f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3b1f6-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3b1f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b1f6-110">Permission type</span></span> | <span data-ttu-id="3b1f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b1f6-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3b1f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b1f6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3b1f6-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="3b1f6-113">Users.Read.All</span></span> |
|<span data-ttu-id="3b1f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b1f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b1f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-115">Not Supported.</span></span>|
|<span data-ttu-id="3b1f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b1f6-116">Application</span></span>|<span data-ttu-id="3b1f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b1f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByPrinter
GET /print/reports/monthlyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="3b1f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1f6-119">Request headers</span></span>
| <span data-ttu-id="3b1f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3b1f6-120">Name</span></span>      |<span data-ttu-id="3b1f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b1f6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b1f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b1f6-122">Authorization</span></span> | <span data-ttu-id="3b1f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b1f6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1f6-125">Request body</span></span>
<span data-ttu-id="3b1f6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b1f6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1f6-127">Response</span></span>
<span data-ttu-id="3b1f6-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b1f6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b1f6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b1f6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1f6-130">Request</span></span>
<span data-ttu-id="3b1f6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b1f6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1f6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByPrinter
```
# <a name="c"></a>[<span data-ttu-id="3b1f6-133">C#</span><span class="sxs-lookup"><span data-stu-id="3b1f6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b1f6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1f6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b1f6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b1f6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3b1f6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1f6-136">Response</span></span>
<span data-ttu-id="3b1f6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-137">The following is an example of the response.</span></span>
><span data-ttu-id="3b1f6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1f6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter",
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
  "description": "List monthlyPrintUsageSummariesByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


