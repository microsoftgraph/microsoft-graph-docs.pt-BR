---
title: 'callRecord: getPstnCalls'
description: Obter log de chamadas PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cb15b70a023fcdf9731b67704329e7dc0d212cc8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563182"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="2624f-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="2624f-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="2624f-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="2624f-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2624f-105">Obter o log de chamadas PSTN como uma coleção de entradas [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) .</span><span class="sxs-lookup"><span data-stu-id="2624f-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="2624f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2624f-106">Permissions</span></span>

<span data-ttu-id="2624f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2624f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2624f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2624f-109">Permission type</span></span>|<span data-ttu-id="2624f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2624f-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2624f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2624f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2624f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2624f-112">Not supported.</span></span> |
| <span data-ttu-id="2624f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2624f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2624f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2624f-114">Not supported.</span></span> |
| <span data-ttu-id="2624f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2624f-115">Application</span></span>                            | <span data-ttu-id="2624f-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2624f-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2624f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2624f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="2624f-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2624f-118">Function parameters</span></span>

<span data-ttu-id="2624f-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2624f-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2624f-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2624f-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2624f-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2624f-121">Parameter</span></span>|<span data-ttu-id="2624f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2624f-122">Type</span></span>|<span data-ttu-id="2624f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2624f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2624f-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="2624f-124">fromDateTime</span></span>|<span data-ttu-id="2624f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2624f-125">DateTimeOffset</span></span>|<span data-ttu-id="2624f-126">Início do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="2624f-126">Start of time range to query.</span></span> <span data-ttu-id="2624f-127">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="2624f-127">UTC, inclusive.</span></span><br/><span data-ttu-id="2624f-128">O intervalo de tempo é baseado na hora de início da chamada.</span><span class="sxs-lookup"><span data-stu-id="2624f-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="2624f-129">ToDateTime</span><span class="sxs-lookup"><span data-stu-id="2624f-129">toDateTime</span></span>|<span data-ttu-id="2624f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2624f-130">DateTimeOffset</span></span>|<span data-ttu-id="2624f-131">Término do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="2624f-131">End of time range to query.</span></span> <span data-ttu-id="2624f-132">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="2624f-132">UTC, inclusive.</span></span>|

> [!IMPORTANT]
> <span data-ttu-id="2624f-133">\* Os valores **fromDateTime** e **ToDateTime** não podem ser mais de um intervalo de datas de 90 dias.</span><span class="sxs-lookup"><span data-stu-id="2624f-133">\* The **fromDateTime** and **toDateTime** values cannot be more than a date range of 90 days.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2624f-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2624f-134">Request headers</span></span>

|<span data-ttu-id="2624f-135">Nome</span><span class="sxs-lookup"><span data-stu-id="2624f-135">Name</span></span>|<span data-ttu-id="2624f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2624f-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2624f-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="2624f-137">Authorization</span></span>|<span data-ttu-id="2624f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2624f-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="2624f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2624f-140">Response</span></span>

<span data-ttu-id="2624f-141">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção de entradas [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2624f-141">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="2624f-142">Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um `@odata.NextLink` com uma URL para consultar a próxima página de entradas de chamada.</span><span class="sxs-lookup"><span data-stu-id="2624f-142">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="2624f-143">A última página no intervalo de datas não tem `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="2624f-143">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="2624f-144">Para obter mais informações, consulte [paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="2624f-144">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="2624f-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2624f-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2624f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2624f-146">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="2624f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2624f-147">Response</span></span>

<span data-ttu-id="2624f-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2624f-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9c4984c7-6c3c-427d-a30c-bd0b2eacee90",
            "callId": "1835317186_112562680@61.221.3.176",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:08.2589935Z",
            "endDateTime": "2019-11-01T00:03:47.2589935Z",
            "duration": 219,
            "charge": 0.00,
            "callType": "user_in",
            "currency": "USD",
            "calleeNumber": "+1234567890",
            "usageCountryCode": "US",
            "tenantCountryCode": "US",
            "connectionCharge": 0.00,
            "callerNumber": "+0123456789",
            "destinationContext": null,
            "destinationName": "United States",
            "conferenceId": null,
            "licenseCapability": "MCOPSTNU",
            "inventoryType": "Subscriber"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="2624f-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="2624f-149">See also</span></span>

* [<span data-ttu-id="2624f-150">Relatório de uso do Microsoft Teams PSTN</span><span class="sxs-lookup"><span data-stu-id="2624f-150">Microsoft Teams PSTN usage report</span></span>](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="2624f-151">Relatório de roteamento direto no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2624f-151">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
