---
title: Listar dailyPrintUsageSummariesByPrinter
description: Recupere uma lista de resumos de uso de impressão diária, agrupados por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4212b6d207e2b4df42492ec3d947cc8de3f01f7f
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848350"
---
# <a name="list-dailyprintusagesummariesbyprinter"></a><span data-ttu-id="41add-103">Listar dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="41add-103">List dailyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="41add-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41add-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41add-105">Recupere uma lista de resumos de uso de impressão diária, agrupados por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="41add-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41add-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41add-106">Permissions</span></span>
<span data-ttu-id="41add-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41add-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="41add-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="41add-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="41add-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41add-110">Permission type</span></span> | <span data-ttu-id="41add-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41add-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="41add-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41add-112">Delegated (work or school account)</span></span>| <span data-ttu-id="41add-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41add-113">Reports.Read.All</span></span> |
|<span data-ttu-id="41add-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41add-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41add-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41add-115">Not Supported.</span></span>|
|<span data-ttu-id="41add-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41add-116">Application</span></span>|<span data-ttu-id="41add-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41add-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41add-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41add-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter
GET /print/reports/dailyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="41add-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41add-119">Request headers</span></span>
| <span data-ttu-id="41add-120">Nome</span><span class="sxs-lookup"><span data-stu-id="41add-120">Name</span></span>      |<span data-ttu-id="41add-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="41add-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41add-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41add-122">Authorization</span></span> | <span data-ttu-id="41add-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41add-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41add-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41add-125">Request body</span></span>
<span data-ttu-id="41add-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41add-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="41add-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="41add-127">Response</span></span>
<span data-ttu-id="41add-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41add-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41add-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41add-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41add-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41add-130">Request</span></span>
<span data-ttu-id="41add-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41add-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41add-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="41add-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter
```
# <a name="c"></a>[<span data-ttu-id="41add-133">C#</span><span class="sxs-lookup"><span data-stu-id="41add-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41add-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41add-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41add-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41add-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41add-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="41add-136">Response</span></span>
<span data-ttu-id="41add-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41add-137">The following is an example of the response.</span></span>
><span data-ttu-id="41add-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41add-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 314

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
  "description": "List dailyPrintUsageSummariesByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


