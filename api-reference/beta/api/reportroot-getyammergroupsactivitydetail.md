---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8dfd26bbc7de0806c7f41286800a9872d3eb9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639016"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="5039e-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="5039e-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5039e-104">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="5039e-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="5039e-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="5039e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="5039e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5039e-106">Permissions</span></span>

<span data-ttu-id="5039e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5039e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5039e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5039e-109">Permission type</span></span>                        | <span data-ttu-id="5039e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5039e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5039e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5039e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5039e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5039e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5039e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5039e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5039e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5039e-114">Not supported.</span></span>                           |
| <span data-ttu-id="5039e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5039e-115">Application</span></span>                            | <span data-ttu-id="5039e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5039e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5039e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5039e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5039e-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5039e-118">Function parameters</span></span>

<span data-ttu-id="5039e-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5039e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5039e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5039e-120">Parameter</span></span> | <span data-ttu-id="5039e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5039e-121">Type</span></span>   | <span data-ttu-id="5039e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5039e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5039e-123">ponto</span><span class="sxs-lookup"><span data-stu-id="5039e-123">period</span></span>    | <span data-ttu-id="5039e-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5039e-124">string</span></span> | <span data-ttu-id="5039e-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5039e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5039e-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5039e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5039e-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5039e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5039e-128">data</span><span class="sxs-lookup"><span data-stu-id="5039e-128">date</span></span>      | <span data-ttu-id="5039e-129">Data</span><span class="sxs-lookup"><span data-stu-id="5039e-129">Date</span></span>   | <span data-ttu-id="5039e-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="5039e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5039e-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="5039e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5039e-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="5039e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5039e-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="5039e-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="5039e-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="5039e-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5039e-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5039e-135">The default output type is text/csv.</span></span> <span data-ttu-id="5039e-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5039e-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5039e-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5039e-137">Request headers</span></span>

| <span data-ttu-id="5039e-138">Nome</span><span class="sxs-lookup"><span data-stu-id="5039e-138">Name</span></span>          | <span data-ttu-id="5039e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5039e-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5039e-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="5039e-140">Authorization</span></span> | <span data-ttu-id="5039e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5039e-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5039e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5039e-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5039e-144">CSV</span><span class="sxs-lookup"><span data-stu-id="5039e-144">CSV</span></span>

<span data-ttu-id="5039e-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5039e-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5039e-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5039e-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5039e-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5039e-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5039e-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5039e-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5039e-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5039e-149">Report Refresh Date</span></span>
- <span data-ttu-id="5039e-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="5039e-150">Group Display Name</span></span>
- <span data-ttu-id="5039e-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="5039e-151">Is Deleted</span></span>
- <span data-ttu-id="5039e-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="5039e-152">Owner Principal Name</span></span>
- <span data-ttu-id="5039e-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="5039e-153">Last Activity Date</span></span>
- <span data-ttu-id="5039e-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="5039e-154">Group Type</span></span>
- <span data-ttu-id="5039e-155">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="5039e-155">Office 365 Connected</span></span>
- <span data-ttu-id="5039e-156">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="5039e-156">Member Count</span></span>
- <span data-ttu-id="5039e-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="5039e-157">Posted Count</span></span>
- <span data-ttu-id="5039e-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="5039e-158">Read Count</span></span>
- <span data-ttu-id="5039e-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="5039e-159">Liked Count</span></span>
- <span data-ttu-id="5039e-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5039e-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5039e-161">JSON</span><span class="sxs-lookup"><span data-stu-id="5039e-161">JSON</span></span>

<span data-ttu-id="5039e-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5039e-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="5039e-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="5039e-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="5039e-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5039e-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5039e-165">CSV</span><span class="sxs-lookup"><span data-stu-id="5039e-165">CSV</span></span>

<span data-ttu-id="5039e-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="5039e-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5039e-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5039e-167">Request</span></span>

<span data-ttu-id="5039e-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5039e-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5039e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="5039e-169">Response</span></span>

<span data-ttu-id="5039e-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5039e-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5039e-171">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5039e-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5039e-172">Basic</span><span class="sxs-lookup"><span data-stu-id="5039e-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5039e-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5039e-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5039e-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5039e-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5039e-175">JSON</span><span class="sxs-lookup"><span data-stu-id="5039e-175">JSON</span></span>

<span data-ttu-id="5039e-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5039e-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5039e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5039e-177">Request</span></span>

<span data-ttu-id="5039e-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5039e-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5039e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="5039e-179">Response</span></span>

<span data-ttu-id="5039e-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5039e-180">The following is an example of the response.</span></span>

> <span data-ttu-id="5039e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5039e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5039e-183">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5039e-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5039e-184">Basic</span><span class="sxs-lookup"><span data-stu-id="5039e-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5039e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5039e-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitydetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
