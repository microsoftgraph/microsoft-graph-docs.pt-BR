---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 85368416acae9a0a55dde1a9c57ad483b7be5e0c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410980"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="52fab-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="52fab-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52fab-104">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="52fab-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="52fab-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="52fab-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="52fab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52fab-106">Permissions</span></span>

<span data-ttu-id="52fab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52fab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52fab-109">Permission type</span></span>                        | <span data-ttu-id="52fab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52fab-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="52fab-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52fab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52fab-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="52fab-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="52fab-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52fab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52fab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52fab-114">Not supported.</span></span>                           |
| <span data-ttu-id="52fab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52fab-115">Application</span></span>                            | <span data-ttu-id="52fab-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="52fab-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="52fab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52fab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="52fab-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="52fab-118">Function parameters</span></span>

<span data-ttu-id="52fab-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="52fab-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="52fab-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52fab-120">Parameter</span></span> | <span data-ttu-id="52fab-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="52fab-121">Type</span></span>   | <span data-ttu-id="52fab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="52fab-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="52fab-123">ponto</span><span class="sxs-lookup"><span data-stu-id="52fab-123">period</span></span>    | <span data-ttu-id="52fab-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52fab-124">string</span></span> | <span data-ttu-id="52fab-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="52fab-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="52fab-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="52fab-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="52fab-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="52fab-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="52fab-128">data</span><span class="sxs-lookup"><span data-stu-id="52fab-128">date</span></span>      | <span data-ttu-id="52fab-129">Data</span><span class="sxs-lookup"><span data-stu-id="52fab-129">Date</span></span>   | <span data-ttu-id="52fab-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="52fab-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="52fab-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="52fab-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="52fab-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="52fab-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="52fab-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="52fab-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="52fab-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="52fab-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="52fab-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="52fab-135">The default output type is text/csv.</span></span> <span data-ttu-id="52fab-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="52fab-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52fab-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52fab-137">Request headers</span></span>

| <span data-ttu-id="52fab-138">Nome</span><span class="sxs-lookup"><span data-stu-id="52fab-138">Name</span></span>          | <span data-ttu-id="52fab-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="52fab-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="52fab-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="52fab-140">Authorization</span></span> | <span data-ttu-id="52fab-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52fab-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="52fab-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="52fab-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="52fab-144">CSV</span><span class="sxs-lookup"><span data-stu-id="52fab-144">CSV</span></span>

<span data-ttu-id="52fab-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="52fab-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="52fab-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="52fab-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="52fab-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="52fab-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="52fab-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="52fab-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="52fab-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="52fab-149">Report Refresh Date</span></span>
- <span data-ttu-id="52fab-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="52fab-150">Group Display Name</span></span>
- <span data-ttu-id="52fab-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="52fab-151">Is Deleted</span></span>
- <span data-ttu-id="52fab-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="52fab-152">Owner Principal Name</span></span>
- <span data-ttu-id="52fab-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="52fab-153">Last Activity Date</span></span>
- <span data-ttu-id="52fab-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="52fab-154">Group Type</span></span>
- <span data-ttu-id="52fab-155">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="52fab-155">Office 365 Connected</span></span>
- <span data-ttu-id="52fab-156">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="52fab-156">Member Count</span></span>
- <span data-ttu-id="52fab-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="52fab-157">Posted Count</span></span>
- <span data-ttu-id="52fab-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="52fab-158">Read Count</span></span>
- <span data-ttu-id="52fab-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="52fab-159">Liked Count</span></span>
- <span data-ttu-id="52fab-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="52fab-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="52fab-161">JSON</span><span class="sxs-lookup"><span data-stu-id="52fab-161">JSON</span></span>

<span data-ttu-id="52fab-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52fab-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="52fab-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="52fab-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="52fab-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52fab-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="52fab-165">CSV</span><span class="sxs-lookup"><span data-stu-id="52fab-165">CSV</span></span>

<span data-ttu-id="52fab-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="52fab-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="52fab-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52fab-167">Request</span></span>

<span data-ttu-id="52fab-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52fab-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="52fab-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="52fab-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52fab-170">C#</span><span class="sxs-lookup"><span data-stu-id="52fab-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52fab-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52fab-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52fab-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52fab-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="52fab-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="52fab-173">Response</span></span>

<span data-ttu-id="52fab-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52fab-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="52fab-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="52fab-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="52fab-176">JSON</span><span class="sxs-lookup"><span data-stu-id="52fab-176">JSON</span></span>

<span data-ttu-id="52fab-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="52fab-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="52fab-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52fab-178">Request</span></span>

<span data-ttu-id="52fab-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52fab-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="52fab-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="52fab-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52fab-181">C#</span><span class="sxs-lookup"><span data-stu-id="52fab-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52fab-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52fab-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52fab-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52fab-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="52fab-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="52fab-184">Response</span></span>

<span data-ttu-id="52fab-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52fab-185">The following is an example of the response.</span></span>

> <span data-ttu-id="52fab-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52fab-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
