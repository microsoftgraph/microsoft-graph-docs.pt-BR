---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c1da1972729e555121bed9bc45ce149e73d53ccc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267449"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="0b73b-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0b73b-103">reportRoot: getEmailActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b73b-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="0b73b-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="0b73b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="0b73b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b73b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b73b-106">Permissions</span></span>

<span data-ttu-id="0b73b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b73b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b73b-109">Permission type</span></span>                        | <span data-ttu-id="0b73b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b73b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b73b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b73b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b73b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b73b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b73b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b73b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b73b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b73b-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b73b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b73b-115">Application</span></span>                            | <span data-ttu-id="0b73b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b73b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b73b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b73b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0b73b-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0b73b-118">Function parameters</span></span>

<span data-ttu-id="0b73b-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0b73b-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0b73b-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0b73b-120">Parameter</span></span> | <span data-ttu-id="0b73b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b73b-121">Type</span></span>   | <span data-ttu-id="0b73b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b73b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b73b-123">ponto</span><span class="sxs-lookup"><span data-stu-id="0b73b-123">period</span></span>    | <span data-ttu-id="0b73b-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b73b-124">string</span></span> | <span data-ttu-id="0b73b-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0b73b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b73b-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0b73b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b73b-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0b73b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0b73b-128">data</span><span class="sxs-lookup"><span data-stu-id="0b73b-128">date</span></span>      | <span data-ttu-id="0b73b-129">Data</span><span class="sxs-lookup"><span data-stu-id="0b73b-129">Date</span></span>   | <span data-ttu-id="0b73b-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="0b73b-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0b73b-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0b73b-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0b73b-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="0b73b-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0b73b-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="0b73b-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0b73b-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0b73b-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="0b73b-135">The default output type is text/csv.</span></span> <span data-ttu-id="0b73b-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0b73b-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b73b-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-137">Request headers</span></span>

| <span data-ttu-id="0b73b-138">Nome</span><span class="sxs-lookup"><span data-stu-id="0b73b-138">Name</span></span>          | <span data-ttu-id="0b73b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b73b-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0b73b-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b73b-140">Authorization</span></span> | <span data-ttu-id="0b73b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b73b-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0b73b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b73b-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0b73b-144">CSV</span><span class="sxs-lookup"><span data-stu-id="0b73b-144">CSV</span></span>

<span data-ttu-id="0b73b-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0b73b-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b73b-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b73b-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0b73b-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b73b-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0b73b-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b73b-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0b73b-149">Report Refresh Date</span></span>
- <span data-ttu-id="0b73b-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="0b73b-150">User Principal Name</span></span>
- <span data-ttu-id="0b73b-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="0b73b-151">Display Name</span></span>
- <span data-ttu-id="0b73b-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="0b73b-152">Is Deleted</span></span>
- <span data-ttu-id="0b73b-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="0b73b-153">Deleted Date</span></span>
- <span data-ttu-id="0b73b-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="0b73b-154">Last Activity Date</span></span>
- <span data-ttu-id="0b73b-155">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="0b73b-155">Send Count</span></span>
- <span data-ttu-id="0b73b-156">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="0b73b-156">Receive Count</span></span>
- <span data-ttu-id="0b73b-157">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="0b73b-157">Read Count</span></span>
- <span data-ttu-id="0b73b-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="0b73b-158">Assigned Products</span></span>
- <span data-ttu-id="0b73b-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0b73b-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0b73b-160">JSON</span><span class="sxs-lookup"><span data-stu-id="0b73b-160">JSON</span></span>

<span data-ttu-id="0b73b-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-161">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="0b73b-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="0b73b-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0b73b-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b73b-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0b73b-164">CSV</span><span class="sxs-lookup"><span data-stu-id="0b73b-164">CSV</span></span>

<span data-ttu-id="0b73b-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="0b73b-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0b73b-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-166">Request</span></span>

<span data-ttu-id="0b73b-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b73b-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0b73b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b73b-168">Response</span></span>

<span data-ttu-id="0b73b-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b73b-170">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="0b73b-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0b73b-171">C#</span><span class="sxs-lookup"><span data-stu-id="0b73b-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b73b-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b73b-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0b73b-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b73b-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="0b73b-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0b73b-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="0b73b-175">JSON</span><span class="sxs-lookup"><span data-stu-id="0b73b-175">JSON</span></span>

<span data-ttu-id="0b73b-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="0b73b-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0b73b-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b73b-177">Request</span></span>

<span data-ttu-id="0b73b-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b73b-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0b73b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b73b-179">Response</span></span>

<span data-ttu-id="0b73b-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b73b-180">The following is an example of the response.</span></span>

> <span data-ttu-id="0b73b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b73b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b73b-183">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0b73b-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0b73b-184">C#</span><span class="sxs-lookup"><span data-stu-id="0b73b-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b73b-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b73b-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0b73b-186">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b73b-186">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityuserdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
