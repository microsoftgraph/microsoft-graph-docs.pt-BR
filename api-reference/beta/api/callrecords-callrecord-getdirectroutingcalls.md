---
title: 'callRecord: getDirectRoutingCalls'
description: Obter um log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a99b776eda23bd1ebaef63bc3f190cb66bd794a7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601108"
---
# <a name="callrecord-getdirectroutingcalls"></a><span data-ttu-id="e2287-103">callRecord: getDirectRoutingCalls</span><span class="sxs-lookup"><span data-stu-id="e2287-103">callRecord: getDirectRoutingCalls</span></span>

<span data-ttu-id="e2287-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e2287-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2287-105">Obter um log de chamadas de roteamento direto como uma coleção de entradas [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) .</span><span class="sxs-lookup"><span data-stu-id="e2287-105">Get a log of direct routing calls as a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2287-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2287-106">Permissions</span></span>

<span data-ttu-id="e2287-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2287-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2287-109">Permission type</span></span>|<span data-ttu-id="e2287-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2287-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2287-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2287-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2287-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2287-112">Not supported.</span></span> |
| <span data-ttu-id="e2287-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2287-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2287-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2287-114">Not supported.</span></span> |
| <span data-ttu-id="e2287-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2287-115">Application</span></span>                            | <span data-ttu-id="e2287-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2287-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2287-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2287-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a><span data-ttu-id="e2287-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2287-118">Request headers</span></span>

|<span data-ttu-id="e2287-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e2287-119">Name</span></span>|<span data-ttu-id="e2287-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2287-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2287-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2287-121">Authorization</span></span>|<span data-ttu-id="e2287-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2287-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="e2287-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e2287-124">Function parameters</span></span>

<span data-ttu-id="e2287-125">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e2287-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e2287-126">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e2287-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e2287-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2287-127">Parameter</span></span>|<span data-ttu-id="e2287-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2287-128">Type</span></span>|<span data-ttu-id="e2287-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2287-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2287-130">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="e2287-130">fromDateTime</span></span>|<span data-ttu-id="e2287-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2287-131">DateTimeOffset</span></span>|<span data-ttu-id="e2287-132">Início do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="e2287-132">Start of time range to query.</span></span> <span data-ttu-id="e2287-133">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="e2287-133">UTC, inclusive.</span></span><br/><span data-ttu-id="e2287-134">O intervalo de tempo é baseado na hora de início da chamada.</span><span class="sxs-lookup"><span data-stu-id="e2287-134">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="e2287-135">ToDateTime</span><span class="sxs-lookup"><span data-stu-id="e2287-135">toDateTime</span></span>|<span data-ttu-id="e2287-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2287-136">DateTimeOffset</span></span>|<span data-ttu-id="e2287-137">Término do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="e2287-137">End of time range to query.</span></span> <span data-ttu-id="e2287-138">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="e2287-138">UTC, inclusive.</span></span>|

## <a name="response"></a><span data-ttu-id="e2287-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2287-139">Response</span></span>

<span data-ttu-id="e2287-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção de entradas [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2287-140">If successful, this function returns a `200 OK` response code and a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="e2287-141">Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um `@odata.NextLink` com uma URL para consultar a próxima página de entradas de chamada.</span><span class="sxs-lookup"><span data-stu-id="e2287-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="e2287-142">A última página no intervalo de datas não tem `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="e2287-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="e2287-143">Para obter mais informações, consulte [paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="e2287-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="e2287-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2287-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2287-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2287-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="e2287-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2287-146">Response</span></span>

<span data-ttu-id="e2287-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2287-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9e8bba57-dc14-533a-a7dd-f0da6575eed1",
            "correlationId": "c98e1515-a937-4b81-b8a8-3992afde64e0",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:25.105Z",
            "inviteDateTime": "2019-11-01T00:00:21.949Z",
            "failureDateTime": "0001-01-01T00:00:00Z",
            "endDateTime": "2019-11-01T00:00:30.105Z",
            "duration": 5,
            "callType": "ByotIn",
            "successfulCall": true,
            "callerNumber": "+12345678***",
            "calleeNumber": "+01234567***",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="e2287-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="e2287-148">See also</span></span>

* <span data-ttu-id="e2287-149">[Relatório de uso do roteamento direto do Microsoft Teams](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) no centro de administração do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e2287-149">[Microsoft Teams direct routing usage report](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) in the Microsoft Teams admin center</span></span>
* <span data-ttu-id="e2287-150">[Painel de integridade para roteamento direto](/MicrosoftTeams/direct-routing-health-dashboard) no centro de administração do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e2287-150">[Health Dashboard for direct routing](/MicrosoftTeams/direct-routing-health-dashboard) in the Microsoft Teams admin center</span></span>
* [<span data-ttu-id="e2287-151">Relatório de chamada PSTN no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2287-151">PSTN call report in Microsoft Graph</span></span>](callrecords-callrecord-getpstncalls.md)