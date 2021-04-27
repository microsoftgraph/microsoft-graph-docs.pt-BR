---
title: 'reports: getPrinterArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora específica.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8a0daedcc8c8b035e6e2ffba7a5a0e49e632f7ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054893"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="24368-103">reports: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="24368-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="24368-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24368-105">Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora [específica.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="24368-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24368-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24368-106">Permissions</span></span>
<span data-ttu-id="24368-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="24368-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="24368-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="24368-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24368-110">Permission type</span></span> | <span data-ttu-id="24368-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24368-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="24368-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24368-112">Delegated (work or school account)</span></span>| <span data-ttu-id="24368-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24368-113">Reports.Read.All</span></span> |
|<span data-ttu-id="24368-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24368-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24368-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24368-115">Not Supported.</span></span>|
|<span data-ttu-id="24368-116">Application</span><span class="sxs-lookup"><span data-stu-id="24368-116">Application</span></span>|<span data-ttu-id="24368-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24368-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24368-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24368-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="24368-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24368-119">Request headers</span></span>
| <span data-ttu-id="24368-120">Nome</span><span class="sxs-lookup"><span data-stu-id="24368-120">Name</span></span>          | <span data-ttu-id="24368-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="24368-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24368-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24368-122">Authorization</span></span> | <span data-ttu-id="24368-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24368-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="24368-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="24368-125">Function parameters</span></span>

| <span data-ttu-id="24368-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="24368-126">Parameter</span></span>     | <span data-ttu-id="24368-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="24368-127">Type</span></span>                 | <span data-ttu-id="24368-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="24368-128">Required?</span></span> | <span data-ttu-id="24368-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="24368-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="24368-130">Sim</span><span class="sxs-lookup"><span data-stu-id="24368-130">Yes</span></span>       | <span data-ttu-id="24368-131">A ID da impressora para a que retornar dados.</span><span class="sxs-lookup"><span data-stu-id="24368-131">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="24368-132">Não</span><span class="sxs-lookup"><span data-stu-id="24368-132">No</span></span>        | <span data-ttu-id="24368-133">A data de início (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="24368-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="24368-134">Não</span><span class="sxs-lookup"><span data-stu-id="24368-134">No</span></span>        | <span data-ttu-id="24368-135">A data de término (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="24368-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="24368-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="24368-136">Response</span></span>
<span data-ttu-id="24368-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24368-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24368-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24368-138">Example</span></span>
<span data-ttu-id="24368-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="24368-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24368-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24368-140">Request</span></span>
<span data-ttu-id="24368-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24368-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a><span data-ttu-id="24368-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="24368-142">Response</span></span>
<span data-ttu-id="24368-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24368-143">The following is an example of the response.</span></span>
><span data-ttu-id="24368-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24368-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

