---
title: Obter printUsageByPrinter
description: Recupere o resumo de uso de uma impressora para um determinado período de tempo.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9ba1d8a3e91298b87813a9f335bb72482a743b82
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516893"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="d6d2d-103">Obter printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="d6d2d-103">Get printUsageByPrinter</span></span>
<span data-ttu-id="d6d2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d6d2d-105">Recupere um resumo de uso para uma [impressora](../resources/printer.md) para um determinado período de tempo.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-105">Retrieve a usage summary for a [printer](../resources/printer.md) for a particular time period.</span></span> <span data-ttu-id="d6d2d-106">Para descrições de cada um dos pontos de extremidade, consulte [printUsageByPrinter](../resources/printUsageByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="d6d2d-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6d2d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6d2d-107">Permissions</span></span>
<span data-ttu-id="d6d2d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6d2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d6d2d-110">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="d6d2d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6d2d-111">Permission type</span></span> | <span data-ttu-id="d6d2d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6d2d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d6d2d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6d2d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d6d2d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6d2d-114">Reports.Read.All</span></span> |
|<span data-ttu-id="d6d2d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6d2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-116">Not Supported.</span></span>|
|<span data-ttu-id="d6d2d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d2d-117">Application</span></span>|<span data-ttu-id="d6d2d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d2d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6d2d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6d2d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6d2d-120">Optional query parameters</span></span>
<span data-ttu-id="d6d2d-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d6d2d-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d6d2d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6d2d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d2d-123">Request headers</span></span>
|<span data-ttu-id="d6d2d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d6d2d-124">Name</span></span>|<span data-ttu-id="d6d2d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d2d-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6d2d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6d2d-126">Authorization</span></span>|<span data-ttu-id="d6d2d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d2d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d2d-129">Request body</span></span>
<span data-ttu-id="d6d2d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d2d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d2d-131">Response</span></span>

<span data-ttu-id="d6d2d-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printUsageByPrinter](../resources/printusagebyprinter.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6d2d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6d2d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6d2d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d2d-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter/{id}
```


### <a name="response"></a><span data-ttu-id="d6d2d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6d2d-135">Response</span></span>
<span data-ttu-id="d6d2d-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6d2d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

