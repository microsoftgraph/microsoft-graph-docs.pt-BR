---
title: 'callRecord: getPstnCalls'
description: Obter log de chamadas PSTN.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 32e130edfde3384036d0f744b2094811c940aa80
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509916"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="6c42e-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="6c42e-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="6c42e-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="6c42e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c42e-105">Obter o log de chamadas PSTN como uma coleção de entradas [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) .</span><span class="sxs-lookup"><span data-stu-id="6c42e-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c42e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c42e-106">Permissions</span></span>

<span data-ttu-id="6c42e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c42e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c42e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c42e-109">Permission type</span></span>|<span data-ttu-id="6c42e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c42e-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c42e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c42e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c42e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c42e-112">Not supported.</span></span> |
| <span data-ttu-id="6c42e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c42e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c42e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c42e-114">Not supported.</span></span> |
| <span data-ttu-id="6c42e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c42e-115">Application</span></span>| <span data-ttu-id="6c42e-116">CallRecords. Read. PstnCalls</span><span class="sxs-lookup"><span data-stu-id="6c42e-116">CallRecords.Read.PstnCalls</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c42e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c42e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="6c42e-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6c42e-118">Function parameters</span></span>

<span data-ttu-id="6c42e-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="6c42e-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6c42e-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="6c42e-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6c42e-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6c42e-121">Parameter</span></span>|<span data-ttu-id="6c42e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c42e-122">Type</span></span>|<span data-ttu-id="6c42e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c42e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c42e-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="6c42e-124">fromDateTime</span></span>|<span data-ttu-id="6c42e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c42e-125">DateTimeOffset</span></span>|<span data-ttu-id="6c42e-126">Início do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="6c42e-126">Start of time range to query.</span></span> <span data-ttu-id="6c42e-127">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="6c42e-127">UTC, inclusive.</span></span><br/><span data-ttu-id="6c42e-128">O intervalo de tempo é baseado na hora de início da chamada.</span><span class="sxs-lookup"><span data-stu-id="6c42e-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="6c42e-129">ToDateTime</span><span class="sxs-lookup"><span data-stu-id="6c42e-129">toDateTime</span></span>|<span data-ttu-id="6c42e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c42e-130">DateTimeOffset</span></span>|<span data-ttu-id="6c42e-131">Término do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="6c42e-131">End of time range to query.</span></span> <span data-ttu-id="6c42e-132">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="6c42e-132">UTC, inclusive.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6c42e-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c42e-133">Request headers</span></span>

|<span data-ttu-id="6c42e-134">Nome</span><span class="sxs-lookup"><span data-stu-id="6c42e-134">Name</span></span>|<span data-ttu-id="6c42e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c42e-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c42e-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c42e-136">Authorization</span></span>|<span data-ttu-id="6c42e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c42e-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="6c42e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c42e-139">Response</span></span>

<span data-ttu-id="6c42e-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção de entradas [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c42e-140">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="6c42e-141">Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um `@odata.NextLink` com uma URL para consultar a próxima página de entradas de chamada.</span><span class="sxs-lookup"><span data-stu-id="6c42e-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="6c42e-142">A última página no intervalo de datas não tem `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="6c42e-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="6c42e-143">Para obter mais informações, consulte [paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="6c42e-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="6c42e-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c42e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c42e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c42e-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="6c42e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c42e-146">Response</span></span>

<span data-ttu-id="6c42e-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6c42e-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6c42e-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="6c42e-148">See also</span></span>

* [<span data-ttu-id="6c42e-149">Relatório de uso do Microsoft Teams PSTN</span><span class="sxs-lookup"><span data-stu-id="6c42e-149">Microsoft Teams PSTN usage report</span></span>](https://docs.microsoft.com/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="6c42e-150">Relatório de roteamento direto no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6c42e-150">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
