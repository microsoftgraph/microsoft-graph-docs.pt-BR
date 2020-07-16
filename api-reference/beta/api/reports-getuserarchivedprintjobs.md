---
title: 'relatórios: getUserArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados para um usuário específico.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 017488e472143d66b48ca33732c0ea1d6aa07475
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845439"
---
# <a name="reports-getuserarchivedprintjobs"></a><span data-ttu-id="834bc-103">relatórios: getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="834bc-103">reports: getUserArchivedPrintJobs</span></span>

<span data-ttu-id="834bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="834bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="834bc-105">Obter uma lista de trabalhos de impressão arquivados para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="834bc-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="834bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="834bc-106">Permissions</span></span>
<span data-ttu-id="834bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="834bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="834bc-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="834bc-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="834bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="834bc-110">Permission type</span></span> | <span data-ttu-id="834bc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="834bc-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="834bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="834bc-112">Delegated (work or school account)</span></span>| <span data-ttu-id="834bc-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="834bc-113">Users.Read.All</span></span> |
|<span data-ttu-id="834bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="834bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="834bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="834bc-115">Not Supported.</span></span>|
|<span data-ttu-id="834bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="834bc-116">Application</span></span>|<span data-ttu-id="834bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="834bc-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="834bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="834bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getUserArchivedPrintJobs
GET /reports/getUserArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="834bc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="834bc-119">Request headers</span></span>
| <span data-ttu-id="834bc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="834bc-120">Name</span></span>          | <span data-ttu-id="834bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="834bc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="834bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="834bc-122">Authorization</span></span> | <span data-ttu-id="834bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="834bc-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="834bc-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="834bc-125">Function Parameters</span></span>

| <span data-ttu-id="834bc-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="834bc-126">Parameter</span></span>     | <span data-ttu-id="834bc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="834bc-127">Type</span></span>                 | <span data-ttu-id="834bc-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="834bc-128">Required?</span></span> | <span data-ttu-id="834bc-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="834bc-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="834bc-130">Sim</span><span class="sxs-lookup"><span data-stu-id="834bc-130">Yes</span></span>       | <span data-ttu-id="834bc-131">A ID do usuário para o qual retornar os dados.</span><span class="sxs-lookup"><span data-stu-id="834bc-131">The ID of the user to return data for.</span></span>                               |
| `periodStart` | `Edm.DateTimeOffset` | <span data-ttu-id="834bc-132">Não</span><span class="sxs-lookup"><span data-stu-id="834bc-132">No</span></span>        | <span data-ttu-id="834bc-133">A data de início (inclusive) para o período de tempo para incluir dados.</span><span class="sxs-lookup"><span data-stu-id="834bc-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `periodEnd`   | `Edm.DateTimeOffset` | <span data-ttu-id="834bc-134">Não</span><span class="sxs-lookup"><span data-stu-id="834bc-134">No</span></span>        | <span data-ttu-id="834bc-135">A data de término (inclusive) para o período de tempo para incluir dados.</span><span class="sxs-lookup"><span data-stu-id="834bc-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="834bc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="834bc-136">Response</span></span>
<span data-ttu-id="834bc-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="834bc-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="834bc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="834bc-138">Example</span></span>
<span data-ttu-id="834bc-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="834bc-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="834bc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="834bc-140">Request</span></span>
<span data-ttu-id="834bc-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="834bc-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getuserarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getUserArchivedPrintJobs(userId={id},periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="834bc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="834bc-142">Response</span></span>
<span data-ttu-id="834bc-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="834bc-143">The following is an example of the response.</span></span>
><span data-ttu-id="834bc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="834bc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "printJob: getUserArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->