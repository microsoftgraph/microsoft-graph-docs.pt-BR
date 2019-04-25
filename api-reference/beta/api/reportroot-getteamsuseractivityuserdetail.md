---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7ca084fbae4ca7714a207364bdf0e9f525a39ff4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545599"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="62543-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="62543-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62543-104">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="62543-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="62543-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62543-105">Permissions</span></span>

<span data-ttu-id="62543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62543-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62543-108">Permission type</span></span>                        | <span data-ttu-id="62543-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62543-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62543-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62543-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62543-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62543-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62543-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62543-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62543-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62543-113">Not supported.</span></span>                           |
| <span data-ttu-id="62543-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62543-114">Application</span></span>                            | <span data-ttu-id="62543-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62543-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="62543-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62543-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="62543-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="62543-117">Function parameters</span></span>

<span data-ttu-id="62543-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="62543-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="62543-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="62543-119">Parameter</span></span> | <span data-ttu-id="62543-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="62543-120">Type</span></span>   | <span data-ttu-id="62543-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="62543-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62543-122">ponto</span><span class="sxs-lookup"><span data-stu-id="62543-122">period</span></span>    | <span data-ttu-id="62543-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62543-123">string</span></span> | <span data-ttu-id="62543-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="62543-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62543-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="62543-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62543-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="62543-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="62543-127">data</span><span class="sxs-lookup"><span data-stu-id="62543-127">date</span></span>      | <span data-ttu-id="62543-128">Data</span><span class="sxs-lookup"><span data-stu-id="62543-128">Date</span></span>   | <span data-ttu-id="62543-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="62543-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="62543-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="62543-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="62543-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="62543-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="62543-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="62543-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="62543-133">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="62543-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="62543-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="62543-134">The default output type is text/csv.</span></span> <span data-ttu-id="62543-135">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="62543-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62543-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62543-136">Request headers</span></span>

| <span data-ttu-id="62543-137">Nome</span><span class="sxs-lookup"><span data-stu-id="62543-137">Name</span></span>          | <span data-ttu-id="62543-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="62543-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="62543-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="62543-139">Authorization</span></span> | <span data-ttu-id="62543-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62543-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62543-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="62543-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="62543-143">CSV</span><span class="sxs-lookup"><span data-stu-id="62543-143">CSV</span></span>

<span data-ttu-id="62543-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="62543-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62543-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="62543-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62543-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="62543-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62543-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="62543-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="62543-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="62543-148">Report Refresh Date</span></span>
- <span data-ttu-id="62543-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="62543-149">User Principal Name</span></span>
- <span data-ttu-id="62543-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="62543-150">Last Activity Date</span></span>
- <span data-ttu-id="62543-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="62543-151">Is Deleted</span></span>
- <span data-ttu-id="62543-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="62543-152">Deleted Date</span></span>
- <span data-ttu-id="62543-153">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="62543-153">Assigned Products</span></span>
- <span data-ttu-id="62543-154">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="62543-154">Team Chat Message Count</span></span>
- <span data-ttu-id="62543-155">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="62543-155">Private Chat Message Count</span></span>
- <span data-ttu-id="62543-156">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="62543-156">Call Count</span></span>
- <span data-ttu-id="62543-157">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="62543-157">Meeting Count</span></span>
- <span data-ttu-id="62543-158">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="62543-158">Has Other Action</span></span>
- <span data-ttu-id="62543-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="62543-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="62543-160">JSON</span><span class="sxs-lookup"><span data-stu-id="62543-160">JSON</span></span>

<span data-ttu-id="62543-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62543-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="62543-162">O tamanho de página padrão para essa solicitação é de 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="62543-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="62543-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62543-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="62543-164">CSV</span><span class="sxs-lookup"><span data-stu-id="62543-164">CSV</span></span>

<span data-ttu-id="62543-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="62543-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="62543-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62543-166">Request</span></span>

<span data-ttu-id="62543-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62543-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="62543-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="62543-168">Response</span></span>

<span data-ttu-id="62543-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62543-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="62543-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="62543-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="62543-171">JSON</span><span class="sxs-lookup"><span data-stu-id="62543-171">JSON</span></span>

<span data-ttu-id="62543-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="62543-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="62543-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62543-173">Request</span></span>

<span data-ttu-id="62543-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62543-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="62543-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="62543-175">Response</span></span>

<span data-ttu-id="62543-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62543-176">The following is an example of the response.</span></span>

> <span data-ttu-id="62543-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62543-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
