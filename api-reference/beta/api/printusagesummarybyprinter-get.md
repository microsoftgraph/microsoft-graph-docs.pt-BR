---
title: Obter printUsageSummaryByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 71bce2c90d9ade62f5d473e2d0e530767e8092fe
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895531"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="9cd78-103">Obter printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="9cd78-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="9cd78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cd78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cd78-105">Recupere o resumo de uso de uma [impressora](../resources/printer.md)para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="9cd78-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="9cd78-106">Para obter descrições de cada um dos pontos de extremidade, consulte [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="9cd78-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cd78-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cd78-107">Permissions</span></span>
<span data-ttu-id="9cd78-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cd78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9cd78-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="9cd78-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9cd78-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cd78-111">Permission type</span></span> | <span data-ttu-id="9cd78-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cd78-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9cd78-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cd78-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9cd78-114">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="9cd78-114">Users.Read.All</span></span> |
|<span data-ttu-id="9cd78-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cd78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd78-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cd78-116">Not Supported.</span></span>|
|<span data-ttu-id="9cd78-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cd78-117">Application</span></span>|<span data-ttu-id="9cd78-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cd78-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cd78-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cd78-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9cd78-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd78-120">Request headers</span></span>
| <span data-ttu-id="9cd78-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9cd78-121">Name</span></span>      |<span data-ttu-id="9cd78-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cd78-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cd78-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cd78-123">Authorization</span></span> | <span data-ttu-id="9cd78-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cd78-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cd78-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd78-126">Request body</span></span>
<span data-ttu-id="9cd78-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cd78-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9cd78-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cd78-128">Response</span></span>
<span data-ttu-id="9cd78-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cd78-129">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cd78-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cd78-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cd78-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd78-131">Request</span></span>
<span data-ttu-id="9cd78-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cd78-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="9cd78-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cd78-133">Response</span></span>
<span data-ttu-id="9cd78-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cd78-134">The following is an example of the response.</span></span>
><span data-ttu-id="9cd78-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cd78-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "2020-02-04T00:00:00.0000000Z",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageSummaryByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->