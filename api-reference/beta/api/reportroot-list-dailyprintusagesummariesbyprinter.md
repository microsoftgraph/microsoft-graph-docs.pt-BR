---
title: Listar dailyPrintUsageSummariesByPrinter
description: Recupere uma lista de resumos de uso de impressão diária, agrupados por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7215770011724c2977785a52364af0e41053519b
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895529"
---
# <a name="list-dailyprintusagesummariesbyprinter"></a><span data-ttu-id="5a465-103">Listar dailyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="5a465-103">List dailyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="5a465-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a465-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a465-105">Recupere uma lista de resumos de uso de impressão diária, agrupados por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="5a465-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a465-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a465-106">Permissions</span></span>
<span data-ttu-id="5a465-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5a465-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="5a465-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5a465-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a465-110">Permission type</span></span> | <span data-ttu-id="5a465-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a465-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5a465-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a465-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5a465-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="5a465-113">Users.Read.All</span></span> |
|<span data-ttu-id="5a465-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a465-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a465-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a465-115">Not Supported.</span></span>|
|<span data-ttu-id="5a465-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a465-116">Application</span></span>|<span data-ttu-id="5a465-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a465-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a465-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a465-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter
GET /print/reports/dailyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="5a465-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a465-119">Request headers</span></span>
| <span data-ttu-id="5a465-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5a465-120">Name</span></span>      |<span data-ttu-id="5a465-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a465-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a465-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a465-122">Authorization</span></span> | <span data-ttu-id="5a465-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a465-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a465-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a465-125">Request body</span></span>
<span data-ttu-id="5a465-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a465-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a465-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a465-127">Response</span></span>
<span data-ttu-id="5a465-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a465-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a465-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a465-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a465-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a465-130">Request</span></span>
<span data-ttu-id="5a465-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a465-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter
```
##### <a name="response"></a><span data-ttu-id="5a465-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a465-132">Response</span></span>
<span data-ttu-id="5a465-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a465-133">The following is an example of the response.</span></span>
><span data-ttu-id="5a465-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a465-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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