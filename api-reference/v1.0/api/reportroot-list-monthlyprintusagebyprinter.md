---
title: Listar monthlyPrintUsageByPrinter
description: Recupere uma lista de resumos de uso de impressão mensal, agrupados por impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 55a9e14f60d58377ace22a1a27927b35e629b835
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516940"
---
# <a name="list-monthlyprintusagebyprinter"></a><span data-ttu-id="e8b03-103">Listar monthlyPrintUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="e8b03-103">List monthlyPrintUsageByPrinter</span></span>
<span data-ttu-id="e8b03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e8b03-105">Recupere uma lista de resumos de uso de impressão mensal, agrupados por [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="e8b03-105">Retrieve a list of monthly print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8b03-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8b03-106">Permissions</span></span>
<span data-ttu-id="e8b03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e8b03-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="e8b03-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e8b03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8b03-110">Permission type</span></span> | <span data-ttu-id="e8b03-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8b03-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e8b03-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8b03-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e8b03-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8b03-113">Reports.Read.All</span></span> |
|<span data-ttu-id="e8b03-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8b03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8b03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8b03-115">Not Supported.</span></span>|
|<span data-ttu-id="e8b03-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8b03-116">Application</span></span>|<span data-ttu-id="e8b03-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8b03-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8b03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b03-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/monthlyPrintUsageByPrinter
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8b03-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8b03-119">Optional query parameters</span></span>
<span data-ttu-id="e8b03-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b03-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8b03-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8b03-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8b03-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b03-122">Request headers</span></span>
|<span data-ttu-id="e8b03-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e8b03-123">Name</span></span>|<span data-ttu-id="e8b03-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8b03-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8b03-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8b03-125">Authorization</span></span>|<span data-ttu-id="e8b03-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8b03-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8b03-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b03-128">Request body</span></span>
<span data-ttu-id="e8b03-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8b03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8b03-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b03-130">Response</span></span>

<span data-ttu-id="e8b03-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printUsageByPrinter](../resources/printusagebyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b03-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByPrinter](../resources/printusagebyprinter.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8b03-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8b03-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8b03-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b03-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/monthlyPrintUsageByPrinter
```


### <a name="response"></a><span data-ttu-id="e8b03-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b03-134">Response</span></span>
<span data-ttu-id="e8b03-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8b03-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByPrinter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

