---
title: 'reports: getGroupArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados para um grupo específico.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8eb6c54e3c4cc62ae3908d456ce832eebe83362f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870749"
---
# <a name="reports-getgrouparchivedprintjobs"></a><span data-ttu-id="d1670-103">reports: getGroupArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="d1670-103">reports: getGroupArchivedPrintJobs</span></span>

<span data-ttu-id="d1670-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1670-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1670-105">Obter uma lista de trabalhos de impressão arquivados para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="d1670-105">Get a list of archived print jobs for a particular group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1670-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d1670-106">Permissions</span></span>
<span data-ttu-id="d1670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d1670-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="d1670-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d1670-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1670-110">Permission type</span></span> | <span data-ttu-id="d1670-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1670-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d1670-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1670-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d1670-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1670-113">Reports.Read.All</span></span> |
|<span data-ttu-id="d1670-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1670-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1670-115">Not Supported.</span></span>|
|<span data-ttu-id="d1670-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1670-116">Application</span></span>|<span data-ttu-id="d1670-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1670-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1670-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1670-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="d1670-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1670-119">Request headers</span></span>
| <span data-ttu-id="d1670-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d1670-120">Name</span></span>          | <span data-ttu-id="d1670-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1670-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d1670-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1670-122">Authorization</span></span> | <span data-ttu-id="d1670-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1670-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="d1670-125">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d1670-125">Function parameters</span></span>

| <span data-ttu-id="d1670-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d1670-126">Parameter</span></span>     | <span data-ttu-id="d1670-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1670-127">Type</span></span>                 | <span data-ttu-id="d1670-128">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="d1670-128">Required?</span></span> | <span data-ttu-id="d1670-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1670-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `groupId`     | `Edm.String`         | <span data-ttu-id="d1670-130">Sim</span><span class="sxs-lookup"><span data-stu-id="d1670-130">Yes</span></span>       | <span data-ttu-id="d1670-131">A ID do grupo para o que retornar dados.</span><span class="sxs-lookup"><span data-stu-id="d1670-131">The ID of the group to return data for.</span></span>                              |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="d1670-132">Não</span><span class="sxs-lookup"><span data-stu-id="d1670-132">No</span></span>        | <span data-ttu-id="d1670-133">A data de início (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="d1670-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="d1670-134">Não</span><span class="sxs-lookup"><span data-stu-id="d1670-134">No</span></span>        | <span data-ttu-id="d1670-135">A data de término (inclusive) do período de tempo a ser incluído.</span><span class="sxs-lookup"><span data-stu-id="d1670-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="d1670-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1670-136">Response</span></span>
<span data-ttu-id="d1670-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1670-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1670-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1670-138">Example</span></span>
<span data-ttu-id="d1670-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d1670-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1670-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1670-140">Request</span></span>
<span data-ttu-id="d1670-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1670-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1670-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1670-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reports-getgrouparchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/getGroupArchivedPrintJobs(groupId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```
# <a name="c"></a>[<span data-ttu-id="d1670-143">C#</span><span class="sxs-lookup"><span data-stu-id="d1670-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reports-getgrouparchivedprintjobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1670-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1670-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reports-getgrouparchivedprintjobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1670-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1670-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reports-getgrouparchivedprintjobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1670-146">Java</span><span class="sxs-lookup"><span data-stu-id="d1670-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reports-getgrouparchivedprintjobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1670-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1670-147">Response</span></span>
<span data-ttu-id="d1670-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1670-148">The following is an example of the response.</span></span>
><span data-ttu-id="d1670-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d1670-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

