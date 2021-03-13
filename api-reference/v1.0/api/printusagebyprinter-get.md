---
title: Obter printUsageByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 21a282d85a8792f88b3392950582be26726c7400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774437"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="fc7ad-103">Obter printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="fc7ad-103">Get printUsageByPrinter</span></span>
<span data-ttu-id="fc7ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc7ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="fc7ad-105">Recupere um resumo de uso para uma [impressora](../resources/printer.md) para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-105">Retrieve a usage summary for a [printer](../resources/printer.md) for a particular time period.</span></span> <span data-ttu-id="fc7ad-106">Para descrições de cada um dos pontos de extremidade, consulte [printUsageByPrinter](../resources/printUsageByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="fc7ad-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc7ad-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="fc7ad-107">Permissions</span></span>
<span data-ttu-id="fc7ad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fc7ad-110">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="fc7ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc7ad-111">Permission type</span></span> | <span data-ttu-id="fc7ad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc7ad-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fc7ad-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc7ad-113">Delegated (work or school account)</span></span>| <span data-ttu-id="fc7ad-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc7ad-114">Reports.Read.All</span></span> |
|<span data-ttu-id="fc7ad-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc7ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc7ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-116">Not Supported.</span></span>|
|<span data-ttu-id="fc7ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc7ad-117">Application</span></span>|<span data-ttu-id="fc7ad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc7ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7ad-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc7ad-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc7ad-120">Optional query parameters</span></span>
<span data-ttu-id="fc7ad-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fc7ad-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fc7ad-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc7ad-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7ad-123">Request headers</span></span>
|<span data-ttu-id="fc7ad-124">Nome</span><span class="sxs-lookup"><span data-stu-id="fc7ad-124">Name</span></span>|<span data-ttu-id="fc7ad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc7ad-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc7ad-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc7ad-126">Authorization</span></span>|<span data-ttu-id="fc7ad-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc7ad-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7ad-129">Request body</span></span>
<span data-ttu-id="fc7ad-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc7ad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7ad-131">Response</span></span>

<span data-ttu-id="fc7ad-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printUsageByPrinter](../resources/printusagebyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc7ad-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc7ad-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc7ad-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7ad-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fc7ad-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter/{id}
```
# <a name="c"></a>[<span data-ttu-id="fc7ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="fc7ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc7ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc7ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc7ad-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc7ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc7ad-139">Java</span><span class="sxs-lookup"><span data-stu-id="fc7ad-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fc7ad-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7ad-140">Response</span></span>
<span data-ttu-id="fc7ad-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fc7ad-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "Date",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

