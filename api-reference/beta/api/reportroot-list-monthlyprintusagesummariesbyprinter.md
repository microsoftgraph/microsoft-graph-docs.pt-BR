---
title: Listar monthlyPrintUsageSummariesByPrinter
description: Recupere uma lista de resumos de uso de impressão mensal, agrupadas por impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6c2bbd30796535d5bf42a919d7b48b32ab4a3ab4
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895524"
---
# <a name="list-monthlyprintusagesummariesbyprinter"></a><span data-ttu-id="64aca-103">Listar monthlyPrintUsageSummariesByPrinter</span><span class="sxs-lookup"><span data-stu-id="64aca-103">List monthlyPrintUsageSummariesByPrinter</span></span>

<span data-ttu-id="64aca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64aca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64aca-105">Recupere uma lista de resumos de uso de impressão mensal, agrupadas por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="64aca-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64aca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64aca-106">Permissions</span></span>
<span data-ttu-id="64aca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64aca-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="64aca-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="64aca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64aca-110">Permission type</span></span> | <span data-ttu-id="64aca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64aca-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="64aca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64aca-112">Delegated (work or school account)</span></span>| <span data-ttu-id="64aca-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="64aca-113">Users.Read.All</span></span> |
|<span data-ttu-id="64aca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64aca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64aca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64aca-115">Not Supported.</span></span>|
|<span data-ttu-id="64aca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64aca-116">Application</span></span>|<span data-ttu-id="64aca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64aca-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64aca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64aca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/monthlyPrintUsageSummariesByPrinter
GET /print/reports/monthlyPrintUsageSummariesByPrinter
```

## <a name="request-headers"></a><span data-ttu-id="64aca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64aca-119">Request headers</span></span>
| <span data-ttu-id="64aca-120">Nome</span><span class="sxs-lookup"><span data-stu-id="64aca-120">Name</span></span>      |<span data-ttu-id="64aca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="64aca-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64aca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64aca-122">Authorization</span></span> | <span data-ttu-id="64aca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64aca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64aca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64aca-125">Request body</span></span>
<span data-ttu-id="64aca-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64aca-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="64aca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64aca-127">Response</span></span>
<span data-ttu-id="64aca-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64aca-128">If successful, this method returns a `200 OK` response code and a collection of [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64aca-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64aca-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64aca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64aca-130">Request</span></span>
<span data-ttu-id="64aca-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64aca-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/monthlyPrintUsageSummariesByPrinter
```
##### <a name="response"></a><span data-ttu-id="64aca-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64aca-132">Response</span></span>
<span data-ttu-id="64aca-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64aca-133">The following is an example of the response.</span></span>
><span data-ttu-id="64aca-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64aca-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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