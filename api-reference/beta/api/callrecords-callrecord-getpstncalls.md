---
title: 'callRecord: getPstnCalls'
description: Obter log de chamadas PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 57f29fdef863671c36f8b9e063c99a370e1173d1
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697190"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="b121c-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="b121c-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="b121c-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="b121c-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b121c-105">Obter log de chamadas PSTN como uma coleção de [entradas pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)</span><span class="sxs-lookup"><span data-stu-id="b121c-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="b121c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b121c-106">Permissions</span></span>

<span data-ttu-id="b121c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b121c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b121c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b121c-109">Permission type</span></span>|<span data-ttu-id="b121c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b121c-110">Permissions (from least to most privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b121c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b121c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b121c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b121c-112">Not supported.</span></span> |
| <span data-ttu-id="b121c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b121c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b121c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b121c-114">Not supported.</span></span> |
| <span data-ttu-id="b121c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b121c-115">Application</span></span>                            | <span data-ttu-id="b121c-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="b121c-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b121c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b121c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="b121c-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b121c-118">Function parameters</span></span>

<span data-ttu-id="b121c-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="b121c-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b121c-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b121c-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b121c-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b121c-121">Parameter</span></span>|<span data-ttu-id="b121c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b121c-122">Type</span></span>|<span data-ttu-id="b121c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b121c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b121c-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="b121c-124">fromDateTime</span></span>|<span data-ttu-id="b121c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b121c-125">DateTimeOffset</span></span>|<span data-ttu-id="b121c-126">Início do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="b121c-126">Start of time range to query.</span></span> <span data-ttu-id="b121c-127">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="b121c-127">UTC, inclusive.</span></span><br/><span data-ttu-id="b121c-128">O intervalo de tempo se baseia na hora de início da chamada.</span><span class="sxs-lookup"><span data-stu-id="b121c-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="b121c-129">toDateTime</span><span class="sxs-lookup"><span data-stu-id="b121c-129">toDateTime</span></span>|<span data-ttu-id="b121c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b121c-130">DateTimeOffset</span></span>|<span data-ttu-id="b121c-131">Fim do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="b121c-131">End of time range to query.</span></span> <span data-ttu-id="b121c-132">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="b121c-132">UTC, inclusive.</span></span>|

> [!IMPORTANT]
> <span data-ttu-id="b121c-133">Os **valores fromDateTime** **e toDateTime** não podem ser mais de um intervalo de datas de 90 dias.</span><span class="sxs-lookup"><span data-stu-id="b121c-133">The **fromDateTime** and **toDateTime** values cannot be more than a date range of 90 days.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b121c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b121c-134">Request headers</span></span>

|<span data-ttu-id="b121c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b121c-135">Name</span></span>|<span data-ttu-id="b121c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b121c-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b121c-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b121c-137">Authorization</span></span>|<span data-ttu-id="b121c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b121c-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b121c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b121c-140">Response</span></span>

<span data-ttu-id="b121c-141">Se tiver êxito, essa função retornará um código de resposta e uma coleção de entradas `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b121c-141">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="b121c-142">Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um com uma URL para consultar a próxima página de entradas `@odata.NextLink` de chamada.</span><span class="sxs-lookup"><span data-stu-id="b121c-142">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="b121c-143">A última página no intervalo de datas não tem `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="b121c-143">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="b121c-144">Para obter mais informações, [consulte paging Microsoft Graph data in your app](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="b121c-144">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="b121c-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b121c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b121c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b121c-146">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="b121c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b121c-147">Response</span></span>

<span data-ttu-id="b121c-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b121c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "inventoryType": "Subscriber",
            "operator": "Microsoft",
            "callDurationSource": "microsoft"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="b121c-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="b121c-149">See also</span></span>

* [<span data-ttu-id="b121c-150">Relatório de uso PSTN do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b121c-150">Microsoft Teams PSTN usage report</span></span>](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="b121c-151">Relatório de roteamento direto no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b121c-151">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
