---
title: 'callRecord: getDirectRoutingCalls'
description: Obter um log de chamadas de roteamento direto.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4fa60bf34d55382ee9a7a04e5b506e92b12a4d75
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313279"
---
# <a name="callrecord-getdirectroutingcalls"></a><span data-ttu-id="39973-103">callRecord: getDirectRoutingCalls</span><span class="sxs-lookup"><span data-stu-id="39973-103">callRecord: getDirectRoutingCalls</span></span>

<span data-ttu-id="39973-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="39973-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39973-105">Obter um log de chamadas de roteamento direto como uma coleção de entradas [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) .</span><span class="sxs-lookup"><span data-stu-id="39973-105">Get a log of direct routing calls as a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="39973-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39973-106">Permissions</span></span>

<span data-ttu-id="39973-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39973-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39973-109">Permission type</span></span>|<span data-ttu-id="39973-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39973-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39973-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39973-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39973-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39973-112">Not supported.</span></span> |
| <span data-ttu-id="39973-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39973-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39973-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39973-114">Not supported.</span></span> |
| <span data-ttu-id="39973-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39973-115">Application</span></span>                            | <span data-ttu-id="39973-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="39973-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39973-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39973-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a><span data-ttu-id="39973-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39973-118">Request headers</span></span>

|<span data-ttu-id="39973-119">Nome</span><span class="sxs-lookup"><span data-stu-id="39973-119">Name</span></span>|<span data-ttu-id="39973-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="39973-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="39973-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39973-121">Authorization</span></span>|<span data-ttu-id="39973-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39973-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="39973-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="39973-124">Function parameters</span></span>

<span data-ttu-id="39973-125">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="39973-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="39973-126">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="39973-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="39973-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="39973-127">Parameter</span></span>|<span data-ttu-id="39973-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="39973-128">Type</span></span>|<span data-ttu-id="39973-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="39973-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39973-130">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="39973-130">fromDateTime</span></span>|<span data-ttu-id="39973-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39973-131">DateTimeOffset</span></span>|<span data-ttu-id="39973-132">Início do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="39973-132">Start of time range to query.</span></span> <span data-ttu-id="39973-133">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="39973-133">UTC, inclusive.</span></span><br/><span data-ttu-id="39973-134">O intervalo de tempo é baseado na hora de início da chamada.</span><span class="sxs-lookup"><span data-stu-id="39973-134">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="39973-135">ToDateTime</span><span class="sxs-lookup"><span data-stu-id="39973-135">toDateTime</span></span>|<span data-ttu-id="39973-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39973-136">DateTimeOffset</span></span>|<span data-ttu-id="39973-137">Término do intervalo de tempo para consulta.</span><span class="sxs-lookup"><span data-stu-id="39973-137">End of time range to query.</span></span> <span data-ttu-id="39973-138">UTC, inclusive.</span><span class="sxs-lookup"><span data-stu-id="39973-138">UTC, inclusive.</span></span>|

## <a name="response"></a><span data-ttu-id="39973-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="39973-139">Response</span></span>

<span data-ttu-id="39973-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção de entradas [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39973-140">If successful, this function returns a `200 OK` response code and a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="39973-141">Se houver mais de 1000 entradas no intervalo de datas, o corpo também incluirá um `@odata.NextLink` com uma URL para consultar a próxima página de entradas de chamada.</span><span class="sxs-lookup"><span data-stu-id="39973-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="39973-142">A última página no intervalo de datas não tem `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="39973-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="39973-143">Para obter mais informações, consulte [paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="39973-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="39973-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39973-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39973-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39973-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="39973-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="39973-146">Response</span></span>

<span data-ttu-id="39973-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="39973-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="39973-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="39973-148">See also</span></span>

* <span data-ttu-id="39973-149">[Relatório de uso do roteamento direto do Microsoft Teams](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) no centro de administração do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="39973-149">[Microsoft Teams direct routing usage report](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) in the Microsoft Teams admin center</span></span>
* <span data-ttu-id="39973-150">[Painel de integridade para roteamento direto](/MicrosoftTeams/direct-routing-health-dashboard) no centro de administração do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="39973-150">[Health Dashboard for direct routing](/MicrosoftTeams/direct-routing-health-dashboard) in the Microsoft Teams admin center</span></span>
* [<span data-ttu-id="39973-151">Relatório de chamada PSTN no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39973-151">PSTN call report in Microsoft Graph</span></span>](callrecords-callrecord-getpstncalls.md)