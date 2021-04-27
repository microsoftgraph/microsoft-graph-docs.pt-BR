---
title: Listar monthlyPrintUsageSummariesByPrinter
description: Recupere uma lista de resumos de uso de impressão mensal, agrupados por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ac8d05c2c89cab203f186727f2680ae0c7e74fe7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054907"
---
# <a name="list-monthlyprintusagesummariesbyprinter"></a><span data-ttu-id="c548a-103">Listar monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="c548a-103">List monthlyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="c548a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c548a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c548a-105">Recupere uma lista de resumos de uso de impressão mensal, agrupados por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="c548a-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c548a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c548a-106">Permissions</span></span>
<span data-ttu-id="c548a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c548a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c548a-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="c548a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c548a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c548a-110">Permission type</span></span> | <span data-ttu-id="c548a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c548a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c548a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c548a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c548a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c548a-113">Reports.Read.All</span></span> |
|<span data-ttu-id="c548a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c548a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c548a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c548a-115">Not Supported.</span></span>|
|<span data-ttu-id="c548a-116">Application</span><span class="sxs-lookup"><span data-stu-id="c548a-116">Application</span></span>|<span data-ttu-id="c548a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c548a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c548a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c548a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByPrinter
GET /print/reports/monthlyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="c548a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c548a-119">Request headers</span></span>
| <span data-ttu-id="c548a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c548a-120">Name</span></span>      |<span data-ttu-id="c548a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c548a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c548a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c548a-122">Authorization</span></span> | <span data-ttu-id="c548a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c548a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c548a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c548a-125">Request body</span></span>
<span data-ttu-id="c548a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c548a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c548a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c548a-127">Response</span></span>
<span data-ttu-id="c548a-128">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c548a-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c548a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c548a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c548a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c548a-130">Request</span></span>
<span data-ttu-id="c548a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c548a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c548a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c548a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoints_5"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByPrinter
```
# <a name="c"></a>[<span data-ttu-id="c548a-133">C#</span><span class="sxs-lookup"><span data-stu-id="c548a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoints-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c548a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c548a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoints-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c548a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c548a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoints-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c548a-136">Java</span><span class="sxs-lookup"><span data-stu-id="c548a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-endpoints-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c548a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c548a-137">Response</span></span>
<span data-ttu-id="c548a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c548a-138">The following is an example of the response.</span></span>
><span data-ttu-id="c548a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c548a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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


