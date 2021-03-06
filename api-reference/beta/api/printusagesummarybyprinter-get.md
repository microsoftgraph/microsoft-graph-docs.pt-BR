---
title: Obter printUsageSummaryByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 8cfda5016861ada120914cc61b19c00081dc5297
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515650"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="4f18c-103">Obter printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="4f18c-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="4f18c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f18c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f18c-105">Recupere o [resumo de](../resources/printer.md)uso de uma impressora para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="4f18c-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="4f18c-106">Para descrições de cada um dos pontos de extremidade, consulte [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="4f18c-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4f18c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f18c-107">Permissions</span></span>
<span data-ttu-id="4f18c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f18c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4f18c-110">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4f18c-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="4f18c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f18c-111">Permission type</span></span> | <span data-ttu-id="4f18c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f18c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4f18c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f18c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4f18c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f18c-114">Reports.Read.All</span></span> |
|<span data-ttu-id="4f18c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f18c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f18c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f18c-116">Not Supported.</span></span>|
|<span data-ttu-id="4f18c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f18c-117">Application</span></span>|<span data-ttu-id="4f18c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f18c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f18c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f18c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monthlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f18c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f18c-120">Optional query parameters</span></span>
<span data-ttu-id="4f18c-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f18c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4f18c-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4f18c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f18c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f18c-123">Request headers</span></span>
| <span data-ttu-id="4f18c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4f18c-124">Name</span></span>      |<span data-ttu-id="4f18c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f18c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f18c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f18c-126">Authorization</span></span> | <span data-ttu-id="4f18c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f18c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f18c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f18c-129">Request body</span></span>
<span data-ttu-id="4f18c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f18c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4f18c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f18c-131">Response</span></span>
<span data-ttu-id="4f18c-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f18c-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f18c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f18c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f18c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f18c-134">Request</span></span>
<span data-ttu-id="4f18c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f18c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f18c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f18c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
# <a name="c"></a>[<span data-ttu-id="4f18c-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f18c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagesummarybyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f18c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f18c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagesummarybyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f18c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f18c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagesummarybyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f18c-140">Java</span><span class="sxs-lookup"><span data-stu-id="4f18c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagesummarybyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4f18c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f18c-141">Response</span></span>
<span data-ttu-id="4f18c-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f18c-142">The following is an example of the response.</span></span>
><span data-ttu-id="4f18c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f18c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

