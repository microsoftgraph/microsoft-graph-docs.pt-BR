---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: eba2f5d05a5571bf7f4fa4cd72d9a945b9936481
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766396"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="129a1-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="129a1-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="129a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="129a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="129a1-105">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="129a1-105">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="129a1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="129a1-106">Permissions</span></span>

<span data-ttu-id="129a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="129a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="129a1-109">Permission type</span></span>                        | <span data-ttu-id="129a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="129a1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="129a1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="129a1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="129a1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="129a1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="129a1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="129a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="129a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="129a1-114">Not supported.</span></span>                           |
| <span data-ttu-id="129a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="129a1-115">Application</span></span>                            | <span data-ttu-id="129a1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="129a1-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="129a1-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="129a1-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="129a1-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="129a1-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="129a1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="129a1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="129a1-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="129a1-120">Function parameters</span></span>

<span data-ttu-id="129a1-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="129a1-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="129a1-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="129a1-122">Parameter</span></span> | <span data-ttu-id="129a1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="129a1-123">Type</span></span>   | <span data-ttu-id="129a1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="129a1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="129a1-125">ponto</span><span class="sxs-lookup"><span data-stu-id="129a1-125">period</span></span>    | <span data-ttu-id="129a1-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="129a1-126">string</span></span> | <span data-ttu-id="129a1-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="129a1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="129a1-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="129a1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="129a1-129">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="129a1-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="129a1-130">data</span><span class="sxs-lookup"><span data-stu-id="129a1-130">date</span></span>      | <span data-ttu-id="129a1-131">Data</span><span class="sxs-lookup"><span data-stu-id="129a1-131">Date</span></span>   | <span data-ttu-id="129a1-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="129a1-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="129a1-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="129a1-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="129a1-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="129a1-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="129a1-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="129a1-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="129a1-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="129a1-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="129a1-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="129a1-137">The default output type is text/csv.</span></span> <span data-ttu-id="129a1-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="129a1-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="129a1-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="129a1-139">Request headers</span></span>

| <span data-ttu-id="129a1-140">Nome</span><span class="sxs-lookup"><span data-stu-id="129a1-140">Name</span></span>          | <span data-ttu-id="129a1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="129a1-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="129a1-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="129a1-142">Authorization</span></span> | <span data-ttu-id="129a1-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="129a1-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="129a1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="129a1-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="129a1-146">CSV</span><span class="sxs-lookup"><span data-stu-id="129a1-146">CSV</span></span>

<span data-ttu-id="129a1-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="129a1-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="129a1-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="129a1-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="129a1-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="129a1-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="129a1-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="129a1-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="129a1-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="129a1-151">Report Refresh Date</span></span>
- <span data-ttu-id="129a1-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="129a1-152">User Principal Name</span></span>
- <span data-ttu-id="129a1-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="129a1-153">Last Activity Date</span></span>
- <span data-ttu-id="129a1-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="129a1-154">Is Deleted</span></span>
- <span data-ttu-id="129a1-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="129a1-155">Deleted Date</span></span>
- <span data-ttu-id="129a1-156">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="129a1-156">Assigned Products</span></span>
- <span data-ttu-id="129a1-157">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="129a1-157">Team Chat Message Count</span></span>
- <span data-ttu-id="129a1-158">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="129a1-158">Private Chat Message Count</span></span>
- <span data-ttu-id="129a1-159">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="129a1-159">Call Count</span></span>
- <span data-ttu-id="129a1-160">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="129a1-160">Meeting Count</span></span>
- <span data-ttu-id="129a1-161">Contagem Organizada de Reuniões</span><span class="sxs-lookup"><span data-stu-id="129a1-161">Meetings Organized Count</span></span>
- <span data-ttu-id="129a1-162">Contagem de Reuniões Atendidas</span><span class="sxs-lookup"><span data-stu-id="129a1-162">Meetings Attended Count</span></span>
- <span data-ttu-id="129a1-163">Contagem Organizada de Reuniões Ad Hoc</span><span class="sxs-lookup"><span data-stu-id="129a1-163">Ad Hoc Meetings Organized Count</span></span>
- <span data-ttu-id="129a1-164">Contagem de Presença de Reuniões Ad Hoc</span><span class="sxs-lookup"><span data-stu-id="129a1-164">Ad Hoc Meetings Attended Count</span></span>
- <span data-ttu-id="129a1-165">Contagem Organizada de Reuniões Agendadas Única</span><span class="sxs-lookup"><span data-stu-id="129a1-165">Scheduled One-time Meetings Organized Count</span></span>
- <span data-ttu-id="129a1-166">Contagem de Reuniões Agendadas Única</span><span class="sxs-lookup"><span data-stu-id="129a1-166">Scheduled One-time Meetings Attended Count</span></span>
- <span data-ttu-id="129a1-167">Contagem Organizada de Reuniões Recorrentes Agendadas</span><span class="sxs-lookup"><span data-stu-id="129a1-167">Scheduled Recurring Meetings Organized Count</span></span>
- <span data-ttu-id="129a1-168">Contagem de reuniões recorrentes agendadas</span><span class="sxs-lookup"><span data-stu-id="129a1-168">Scheduled Recurring Meetings Attended Count</span></span>
- <span data-ttu-id="129a1-169">Duração do Áudio</span><span class="sxs-lookup"><span data-stu-id="129a1-169">Audio Duration</span></span>
- <span data-ttu-id="129a1-170">Duração do vídeo</span><span class="sxs-lookup"><span data-stu-id="129a1-170">Video Duration</span></span>
- <span data-ttu-id="129a1-171">Duração do Compartilhamento de Tela</span><span class="sxs-lookup"><span data-stu-id="129a1-171">Screen Share Duration</span></span>
- <span data-ttu-id="129a1-172">Duração do áudio em segundos</span><span class="sxs-lookup"><span data-stu-id="129a1-172">Audio Duration In Seconds</span></span>
- <span data-ttu-id="129a1-173">Duração do vídeo em segundos</span><span class="sxs-lookup"><span data-stu-id="129a1-173">Video Duration In Seconds</span></span>
- <span data-ttu-id="129a1-174">Duração do compartilhamento de tela em segundos</span><span class="sxs-lookup"><span data-stu-id="129a1-174">Screen Share Duration In Seconds</span></span>
- <span data-ttu-id="129a1-175">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="129a1-175">Has Other Action</span></span>
- <span data-ttu-id="129a1-176">É Licenciado</span><span class="sxs-lookup"><span data-stu-id="129a1-176">Is Licensed</span></span>
- <span data-ttu-id="129a1-177">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="129a1-177">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="129a1-178">JSON</span><span class="sxs-lookup"><span data-stu-id="129a1-178">JSON</span></span>

<span data-ttu-id="129a1-179">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="129a1-179">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="129a1-180">O tamanho padrão da página para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="129a1-180">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="129a1-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="129a1-181">Example</span></span>

### <a name="csv"></a><span data-ttu-id="129a1-182">CSV</span><span class="sxs-lookup"><span data-stu-id="129a1-182">CSV</span></span>

<span data-ttu-id="129a1-183">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="129a1-183">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="129a1-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="129a1-184">Request</span></span>

<span data-ttu-id="129a1-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="129a1-185">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="129a1-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="129a1-186">Response</span></span>

<span data-ttu-id="129a1-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="129a1-187">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="129a1-188">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="129a1-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Meetings Organized Count,Meetings Attended Count,Ad Hoc Meetings Organized Count,Ad Hoc Meetings Attended Count,Scheduled One-time Meetings Organized Count,Scheduled One-time Meetings Attended Count,Scheduled Recurring Meetings Organized Count,Scheduled Recurring Meetings Attended Count,Audio Duration,Video Duration,Screen Share Duration,Audio Duration In Seconds,Video Duration In Seconds,Screen Share Duration In Seconds,Has Other Action,Is Licensed,Report Period
```

### <a name="json"></a><span data-ttu-id="129a1-189">JSON</span><span class="sxs-lookup"><span data-stu-id="129a1-189">JSON</span></span>

<span data-ttu-id="129a1-190">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="129a1-190">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="129a1-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="129a1-191">Request</span></span>

<span data-ttu-id="129a1-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="129a1-192">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="129a1-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="129a1-193">Response</span></span>

<span data-ttu-id="129a1-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="129a1-194">The following is an example of the response.</span></span>

> <span data-ttu-id="129a1-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="129a1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isLicensed": true, 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "meetingsOrganizedCount": 0, 
      "meetingsAttendedCount": 0, 
      "adHocMeetingsOrganizedCount": 0, 
      "adHocMeetingsAttendedCount": 0, 
      "scheduledOneTimeMeetingsOrganizedCount": 0, 
      "scheduledOneTimeMeetingsAttendedCount": 0, 
      "scheduledRecurringMeetingsOrganizedCount": 0, 
      "scheduledRecurringMeetingsAttendedCount": 0, 
      "audioDuration": 00:00:00, 
      "videoDuration": 00:00:00, 
      "screenShareDuration": 00:00:00, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


