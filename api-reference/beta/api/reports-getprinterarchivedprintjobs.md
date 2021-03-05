---
title: 'reports: getPrinterArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora específica.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: daf0acf2ab9bc285d05aae9f3b875ffc6f329b03
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472399"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="8cc62-103">reports: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="8cc62-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="8cc62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc62-105">Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora [específica.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="8cc62-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc62-106">Permissions</span></span>
<span data-ttu-id="8cc62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8cc62-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="8cc62-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8cc62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc62-110">Permission type</span></span> | <span data-ttu-id="8cc62-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc62-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8cc62-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc62-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8cc62-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cc62-113">Reports.Read.All</span></span> |
|<span data-ttu-id="8cc62-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc62-115">Not Supported.</span></span>|
|<span data-ttu-id="8cc62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc62-116">Application</span></span>|<span data-ttu-id="8cc62-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc62-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="8cc62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc62-119">Request headers</span></span>
| <span data-ttu-id="8cc62-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc62-120">Name</span></span>          | <span data-ttu-id="8cc62-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc62-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8cc62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc62-122">Authorization</span></span> | <span data-ttu-id="8cc62-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc62-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="8cc62-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8cc62-125">Function parameters</span></span>

| <span data-ttu-id="8cc62-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8cc62-126">Parameter</span></span>     | <span data-ttu-id="8cc62-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc62-127">Type</span></span>                 | <span data-ttu-id="8cc62-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="8cc62-128">Required?</span></span> | <span data-ttu-id="8cc62-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc62-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="8cc62-130">Sim</span><span class="sxs-lookup"><span data-stu-id="8cc62-130">Yes</span></span>       | <span data-ttu-id="8cc62-131">A ID da impressora para a que retornar dados.</span><span class="sxs-lookup"><span data-stu-id="8cc62-131">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="8cc62-132">Não</span><span class="sxs-lookup"><span data-stu-id="8cc62-132">No</span></span>        | <span data-ttu-id="8cc62-133">A data de início (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="8cc62-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="8cc62-134">Não</span><span class="sxs-lookup"><span data-stu-id="8cc62-134">No</span></span>        | <span data-ttu-id="8cc62-135">A data de término (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="8cc62-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="8cc62-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc62-136">Response</span></span>
<span data-ttu-id="8cc62-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc62-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc62-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc62-138">Example</span></span>
<span data-ttu-id="8cc62-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8cc62-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cc62-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc62-140">Request</span></span>
<span data-ttu-id="8cc62-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc62-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a><span data-ttu-id="8cc62-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc62-142">Response</span></span>
<span data-ttu-id="8cc62-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc62-143">The following is an example of the response.</span></span>
><span data-ttu-id="8cc62-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc62-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

