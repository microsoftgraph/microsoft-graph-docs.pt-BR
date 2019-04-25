---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a8df675d76f554fc61737cc49942652772650f97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545541"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="d39e0-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d39e0-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d39e0-104">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="d39e0-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="d39e0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="d39e0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="d39e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d39e0-106">Permissions</span></span>

<span data-ttu-id="d39e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d39e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d39e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d39e0-109">Permission type</span></span>                        | <span data-ttu-id="d39e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d39e0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d39e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d39e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d39e0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d39e0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d39e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d39e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d39e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d39e0-114">Not supported.</span></span>                           |
| <span data-ttu-id="d39e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d39e0-115">Application</span></span>                            | <span data-ttu-id="d39e0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d39e0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d39e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d39e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d39e0-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d39e0-118">Function parameters</span></span>

<span data-ttu-id="d39e0-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d39e0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d39e0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d39e0-120">Parameter</span></span> | <span data-ttu-id="d39e0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d39e0-121">Type</span></span>   | <span data-ttu-id="d39e0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d39e0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d39e0-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d39e0-123">period</span></span>    | <span data-ttu-id="d39e0-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d39e0-124">string</span></span> | <span data-ttu-id="d39e0-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d39e0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d39e0-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d39e0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d39e0-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d39e0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d39e0-128">data</span><span class="sxs-lookup"><span data-stu-id="d39e0-128">date</span></span>      | <span data-ttu-id="d39e0-129">Data</span><span class="sxs-lookup"><span data-stu-id="d39e0-129">Date</span></span>   | <span data-ttu-id="d39e0-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="d39e0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d39e0-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d39e0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d39e0-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="d39e0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d39e0-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="d39e0-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d39e0-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="d39e0-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d39e0-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d39e0-135">The default output type is text/csv.</span></span> <span data-ttu-id="d39e0-136">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d39e0-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d39e0-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d39e0-137">Request headers</span></span>

| <span data-ttu-id="d39e0-138">Nome</span><span class="sxs-lookup"><span data-stu-id="d39e0-138">Name</span></span>          | <span data-ttu-id="d39e0-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d39e0-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d39e0-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d39e0-140">Authorization</span></span> | <span data-ttu-id="d39e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d39e0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d39e0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39e0-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d39e0-144">CSV</span><span class="sxs-lookup"><span data-stu-id="d39e0-144">CSV</span></span>

<span data-ttu-id="d39e0-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d39e0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d39e0-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d39e0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d39e0-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d39e0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d39e0-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d39e0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d39e0-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d39e0-149">Report Refresh Date</span></span>
- <span data-ttu-id="d39e0-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="d39e0-150">Group Display Name</span></span>
- <span data-ttu-id="d39e0-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="d39e0-151">Is Deleted</span></span>
- <span data-ttu-id="d39e0-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="d39e0-152">Owner Principal Name</span></span>
- <span data-ttu-id="d39e0-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="d39e0-153">Last Activity Date</span></span>
- <span data-ttu-id="d39e0-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="d39e0-154">Group Type</span></span>
- <span data-ttu-id="d39e0-155">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="d39e0-155">Office 365 Connected</span></span>
- <span data-ttu-id="d39e0-156">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="d39e0-156">Member Count</span></span>
- <span data-ttu-id="d39e0-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="d39e0-157">Posted Count</span></span>
- <span data-ttu-id="d39e0-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="d39e0-158">Read Count</span></span>
- <span data-ttu-id="d39e0-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="d39e0-159">Liked Count</span></span>
- <span data-ttu-id="d39e0-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d39e0-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d39e0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="d39e0-161">JSON</span></span>

<span data-ttu-id="d39e0-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d39e0-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="d39e0-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="d39e0-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d39e0-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d39e0-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d39e0-165">CSV</span><span class="sxs-lookup"><span data-stu-id="d39e0-165">CSV</span></span>

<span data-ttu-id="d39e0-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d39e0-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d39e0-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d39e0-167">Request</span></span>

<span data-ttu-id="d39e0-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d39e0-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d39e0-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39e0-169">Response</span></span>

<span data-ttu-id="d39e0-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d39e0-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d39e0-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d39e0-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="d39e0-172">JSON</span><span class="sxs-lookup"><span data-stu-id="d39e0-172">JSON</span></span>

<span data-ttu-id="d39e0-173">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d39e0-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d39e0-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d39e0-174">Request</span></span>

<span data-ttu-id="d39e0-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d39e0-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d39e0-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39e0-176">Response</span></span>

<span data-ttu-id="d39e0-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d39e0-177">The following is an example of the response.</span></span>

> <span data-ttu-id="d39e0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d39e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
