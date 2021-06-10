---
title: Obter printUsageByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 2789109eeab11a00cd49d9c03163b6b224725e80
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869874"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="4ea8e-103">Obter printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="4ea8e-103">Get printUsageByPrinter</span></span>

<span data-ttu-id="4ea8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea8e-105">Recupere o [resumo de](../resources/printer.md)uso de uma impressora para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span>

<span data-ttu-id="4ea8e-106">Para descrições de cada um dos pontos de extremidade, consulte [printUsageByPrinter](../resources/printUsageByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="4ea8e-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea8e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ea8e-107">Permissions</span></span>
<span data-ttu-id="4ea8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ea8e-110">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="4ea8e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ea8e-111">Permission type</span></span> | <span data-ttu-id="4ea8e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ea8e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ea8e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ea8e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4ea8e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ea8e-114">Reports.Read.All</span></span> |
|<span data-ttu-id="4ea8e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ea8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea8e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-116">Not Supported.</span></span>|
|<span data-ttu-id="4ea8e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ea8e-117">Application</span></span>|<span data-ttu-id="4ea8e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea8e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea8e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
GET /print/reports/dailyPrintUsageByPrinter/{id}
GET /print/reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ea8e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ea8e-120">Optional query parameters</span></span>
<span data-ttu-id="4ea8e-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ea8e-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ea8e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ea8e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea8e-123">Request headers</span></span>
| <span data-ttu-id="4ea8e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4ea8e-124">Name</span></span>      |<span data-ttu-id="4ea8e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea8e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ea8e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea8e-126">Authorization</span></span> | <span data-ttu-id="4ea8e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ea8e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea8e-129">Request body</span></span>
<span data-ttu-id="4ea8e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ea8e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea8e-131">Response</span></span>
<span data-ttu-id="4ea8e-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printUsageByPrinter](../resources/printUsageByPrinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printUsageByPrinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ea8e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ea8e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ea8e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea8e-134">Request</span></span>
<span data-ttu-id="4ea8e-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ea8e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea8e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageByPrinter",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByPrinter/016b5565-3bbf-4067-b9ff-4d68167eb1a6
```
# <a name="c"></a>[<span data-ttu-id="4ea8e-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ea8e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea8e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea8e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea8e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea8e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ea8e-140">Java</span><span class="sxs-lookup"><span data-stu-id="4ea8e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4ea8e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea8e-141">Response</span></span>
<span data-ttu-id="4ea8e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-142">The following is an example of the response.</span></span>
><span data-ttu-id="4ea8e-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4ea8e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
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
  "description": "Get printUsageByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

