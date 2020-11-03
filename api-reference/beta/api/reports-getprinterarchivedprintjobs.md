---
title: 'relatórios: getPrinterArchivedPrintJobs'
description: Obtenha uma lista de trabalhos de impressão arquivados que foram enfileirados para determinada impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a06f20d8de1fc6f1be72e382beaf01158529f260
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848237"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="4451d-103">relatórios: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="4451d-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="4451d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4451d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4451d-105">Obtenha uma lista de trabalhos de impressão arquivados que foram enfileirados para determinada [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="4451d-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4451d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4451d-106">Permissions</span></span>
<span data-ttu-id="4451d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4451d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4451d-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="4451d-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4451d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4451d-110">Permission type</span></span> | <span data-ttu-id="4451d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4451d-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4451d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4451d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4451d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4451d-113">Reports.Read.All</span></span> |
|<span data-ttu-id="4451d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4451d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4451d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4451d-115">Not Supported.</span></span>|
|<span data-ttu-id="4451d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4451d-116">Application</span></span>|<span data-ttu-id="4451d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4451d-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4451d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4451d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs
GET /reports/getPrinterArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="4451d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4451d-119">Request headers</span></span>
| <span data-ttu-id="4451d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4451d-120">Name</span></span>          | <span data-ttu-id="4451d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4451d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4451d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4451d-122">Authorization</span></span> | <span data-ttu-id="4451d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4451d-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="4451d-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4451d-125">Function parameters</span></span>

| <span data-ttu-id="4451d-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4451d-126">Parameter</span></span>     | <span data-ttu-id="4451d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4451d-127">Type</span></span>                 | <span data-ttu-id="4451d-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="4451d-128">Required?</span></span> | <span data-ttu-id="4451d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4451d-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="4451d-130">Sim</span><span class="sxs-lookup"><span data-stu-id="4451d-130">Yes</span></span>       | <span data-ttu-id="4451d-131">A ID da impressora para a qual retornar os dados.</span><span class="sxs-lookup"><span data-stu-id="4451d-131">The ID of the printer to return data for.</span></span>                            |
| `periodStart` | `Edm.DateTimeOffset` | <span data-ttu-id="4451d-132">Não</span><span class="sxs-lookup"><span data-stu-id="4451d-132">No</span></span>        | <span data-ttu-id="4451d-133">A data de início (inclusive) para o período de tempo para incluir dados.</span><span class="sxs-lookup"><span data-stu-id="4451d-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `periodEnd`   | `Edm.DateTimeOffset` | <span data-ttu-id="4451d-134">Não</span><span class="sxs-lookup"><span data-stu-id="4451d-134">No</span></span>        | <span data-ttu-id="4451d-135">A data de término (inclusive) para o período de tempo para incluir dados.</span><span class="sxs-lookup"><span data-stu-id="4451d-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="4451d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4451d-136">Response</span></span>
<span data-ttu-id="4451d-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4451d-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4451d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4451d-138">Example</span></span>
<span data-ttu-id="4451d-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4451d-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4451d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4451d-140">Request</span></span>
<span data-ttu-id="4451d-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4451d-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="4451d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4451d-142">Response</span></span>
<span data-ttu-id="4451d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4451d-143">The following is an example of the response.</span></span>
><span data-ttu-id="4451d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4451d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getPrinterArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

