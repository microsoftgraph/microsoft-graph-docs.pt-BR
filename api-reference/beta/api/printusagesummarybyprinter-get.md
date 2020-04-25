---
title: Obter printUsageSummaryByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: ceccd866e4ba8e19f2c4e93ff8e06e9da700cc47
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812559"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="d2a6e-103">Obter printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="d2a6e-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="d2a6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a6e-105">Recupere o resumo de uso de uma [impressora](../resources/printer.md)para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="d2a6e-106">Para obter descrições de cada um dos pontos de extremidade, consulte [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="d2a6e-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a6e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2a6e-107">Permissions</span></span>
<span data-ttu-id="d2a6e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2a6e-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d2a6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2a6e-111">Permission type</span></span> | <span data-ttu-id="d2a6e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d2a6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d2a6e-114">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2a6e-114">Users.Read.All</span></span> |
|<span data-ttu-id="d2a6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2a6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2a6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-116">Not Supported.</span></span>|
|<span data-ttu-id="d2a6e-117">Application</span><span class="sxs-lookup"><span data-stu-id="d2a6e-117">Application</span></span>|<span data-ttu-id="d2a6e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2a6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a6e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2a6e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d2a6e-120">Optional query parameters</span></span>
<span data-ttu-id="d2a6e-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d2a6e-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d2a6e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2a6e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a6e-123">Request headers</span></span>
| <span data-ttu-id="d2a6e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d2a6e-124">Name</span></span>      |<span data-ttu-id="d2a6e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a6e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2a6e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2a6e-126">Authorization</span></span> | <span data-ttu-id="d2a6e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2a6e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a6e-129">Request body</span></span>
<span data-ttu-id="d2a6e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2a6e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a6e-131">Response</span></span>
<span data-ttu-id="d2a6e-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2a6e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2a6e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2a6e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a6e-134">Request</span></span>
<span data-ttu-id="d2a6e-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="d2a6e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a6e-136">Response</span></span>
<span data-ttu-id="d2a6e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-137">The following is an example of the response.</span></span>
><span data-ttu-id="d2a6e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2a6e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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