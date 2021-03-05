---
title: 'reports: getGroupArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados para um grupo específico.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 98e208816a2415f176407d1d76194046c0284250
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470806"
---
# <a name="reports-getgrouparchivedprintjobs"></a><span data-ttu-id="0d3c1-103">reports: getGroupArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="0d3c1-103">reports: getGroupArchivedPrintJobs</span></span>

<span data-ttu-id="0d3c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d3c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d3c1-105">Obter uma lista de trabalhos de impressão arquivados para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-105">Get a list of archived print jobs for a particular group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d3c1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d3c1-106">Permissions</span></span>
<span data-ttu-id="0d3c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0d3c1-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0d3c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d3c1-110">Permission type</span></span> | <span data-ttu-id="0d3c1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d3c1-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0d3c1-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d3c1-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0d3c1-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d3c1-113">Reports.Read.All</span></span> |
|<span data-ttu-id="0d3c1-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d3c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d3c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-115">Not Supported.</span></span>|
|<span data-ttu-id="0d3c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d3c1-116">Application</span></span>|<span data-ttu-id="0d3c1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d3c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d3c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="0d3c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3c1-119">Request headers</span></span>
| <span data-ttu-id="0d3c1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0d3c1-120">Name</span></span>          | <span data-ttu-id="0d3c1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3c1-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0d3c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d3c1-122">Authorization</span></span> | <span data-ttu-id="0d3c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="0d3c1-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0d3c1-125">Function parameters</span></span>

| <span data-ttu-id="0d3c1-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0d3c1-126">Parameter</span></span>     | <span data-ttu-id="0d3c1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d3c1-127">Type</span></span>                 | <span data-ttu-id="0d3c1-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="0d3c1-128">Required?</span></span> | <span data-ttu-id="0d3c1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3c1-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `groupId`     | `Edm.String`         | <span data-ttu-id="0d3c1-130">Sim</span><span class="sxs-lookup"><span data-stu-id="0d3c1-130">Yes</span></span>       | <span data-ttu-id="0d3c1-131">A ID do grupo para o que retornar dados.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-131">The ID of the group to return data for.</span></span>                              |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="0d3c1-132">Não</span><span class="sxs-lookup"><span data-stu-id="0d3c1-132">No</span></span>        | <span data-ttu-id="0d3c1-133">A data de início (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="0d3c1-134">Não</span><span class="sxs-lookup"><span data-stu-id="0d3c1-134">No</span></span>        | <span data-ttu-id="0d3c1-135">A data de término (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="0d3c1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3c1-136">Response</span></span>
<span data-ttu-id="0d3c1-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d3c1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d3c1-138">Example</span></span>
<span data-ttu-id="0d3c1-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0d3c1-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3c1-140">Request</span></span>
<span data-ttu-id="0d3c1-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getgrouparchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getGroupArchivedPrintJobs(groupId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a><span data-ttu-id="0d3c1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3c1-142">Response</span></span>
<span data-ttu-id="0d3c1-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-143">The following is an example of the response.</span></span>
><span data-ttu-id="0d3c1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "printJob: getGroupArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

