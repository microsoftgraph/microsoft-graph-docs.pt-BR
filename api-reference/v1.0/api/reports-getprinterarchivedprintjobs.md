---
title: 'reports: getPrinterArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora específica.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7e5788016efded3975fe77f4028ecd48b6bbde54
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516936"
---
# <a name="reportroot-getprinterarchivedprintjobs"></a><span data-ttu-id="d8e1e-103">reportRoot: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="d8e1e-103">reportRoot: getPrinterArchivedPrintJobs</span></span>
<span data-ttu-id="d8e1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8e1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d8e1e-105">Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora [específica.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="d8e1e-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8e1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8e1e-106">Permissions</span></span>
<span data-ttu-id="d8e1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d8e1e-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d8e1e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8e1e-110">Permission type</span></span> | <span data-ttu-id="d8e1e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8e1e-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d8e1e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8e1e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d8e1e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8e1e-113">Reports.Read.All</span></span> |
|<span data-ttu-id="d8e1e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8e1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e1e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-115">Not Supported.</span></span>|
|<span data-ttu-id="d8e1e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8e1e-116">Application</span></span>|<span data-ttu-id="d8e1e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e1e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8e1e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getPrinterArchivedPrintJobs
```

## <a name="function-parameters"></a><span data-ttu-id="d8e1e-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d8e1e-119">Function parameters</span></span>

| <span data-ttu-id="d8e1e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8e1e-120">Parameter</span></span>     | <span data-ttu-id="d8e1e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8e1e-121">Type</span></span>                 | <span data-ttu-id="d8e1e-122">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="d8e1e-122">Required?</span></span> | <span data-ttu-id="d8e1e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e1e-123">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="d8e1e-124">Sim</span><span class="sxs-lookup"><span data-stu-id="d8e1e-124">Yes</span></span>       | <span data-ttu-id="d8e1e-125">A ID da impressora para a que retornar dados.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-125">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="d8e1e-126">Não</span><span class="sxs-lookup"><span data-stu-id="d8e1e-126">No</span></span>        | <span data-ttu-id="d8e1e-127">A data de início (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-127">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="d8e1e-128">Não</span><span class="sxs-lookup"><span data-stu-id="d8e1e-128">No</span></span>        | <span data-ttu-id="d8e1e-129">A data de término (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-129">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="request-headers"></a><span data-ttu-id="d8e1e-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e1e-130">Request headers</span></span>
|<span data-ttu-id="d8e1e-131">Nome</span><span class="sxs-lookup"><span data-stu-id="d8e1e-131">Name</span></span>|<span data-ttu-id="d8e1e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e1e-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d8e1e-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8e1e-133">Authorization</span></span>|<span data-ttu-id="d8e1e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e1e-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e1e-136">Request body</span></span>
<span data-ttu-id="d8e1e-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8e1e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8e1e-138">Response</span></span>

<span data-ttu-id="d8e1e-139">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-139">If successful, this function returns a `200 OK` response code and a [archivedPrintJob](../resources/archivedprintjob.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8e1e-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d8e1e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8e1e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e1e-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getprinterarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```


### <a name="response"></a><span data-ttu-id="d8e1e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8e1e-142">Response</span></span>
<span data-ttu-id="d8e1e-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d8e1e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.archivedPrintJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "fe6ff85a-f0d3-4c4f-aec6-b9d5154356a1",
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

