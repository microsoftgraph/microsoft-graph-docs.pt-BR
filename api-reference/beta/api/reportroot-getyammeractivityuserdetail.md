---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8673ee95326a02c5f9d18a25cdf1ae67b09d3ce4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639149"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="906d2-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="906d2-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906d2-104">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="906d2-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="906d2-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="906d2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="906d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="906d2-106">Permissions</span></span>

<span data-ttu-id="906d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="906d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="906d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="906d2-109">Permission type</span></span>                        | <span data-ttu-id="906d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="906d2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="906d2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="906d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="906d2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="906d2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="906d2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="906d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="906d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="906d2-114">Not supported.</span></span>                           |
| <span data-ttu-id="906d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="906d2-115">Application</span></span>                            | <span data-ttu-id="906d2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="906d2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="906d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="906d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="906d2-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="906d2-118">Function parameters</span></span>

<span data-ttu-id="906d2-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="906d2-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="906d2-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="906d2-120">Parameter</span></span> | <span data-ttu-id="906d2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="906d2-121">Type</span></span>   | <span data-ttu-id="906d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="906d2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="906d2-123">ponto</span><span class="sxs-lookup"><span data-stu-id="906d2-123">period</span></span>    | <span data-ttu-id="906d2-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="906d2-124">string</span></span> | <span data-ttu-id="906d2-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="906d2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="906d2-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="906d2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="906d2-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="906d2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="906d2-128">data</span><span class="sxs-lookup"><span data-stu-id="906d2-128">date</span></span>      | <span data-ttu-id="906d2-129">Data</span><span class="sxs-lookup"><span data-stu-id="906d2-129">Date</span></span>   | <span data-ttu-id="906d2-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="906d2-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="906d2-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="906d2-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="906d2-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="906d2-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="906d2-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="906d2-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="906d2-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="906d2-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="906d2-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="906d2-135">The default output type is text/csv.</span></span> <span data-ttu-id="906d2-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="906d2-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="906d2-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="906d2-137">Request headers</span></span>

| <span data-ttu-id="906d2-138">Nome</span><span class="sxs-lookup"><span data-stu-id="906d2-138">Name</span></span>          | <span data-ttu-id="906d2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="906d2-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="906d2-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="906d2-140">Authorization</span></span> | <span data-ttu-id="906d2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="906d2-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="906d2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="906d2-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="906d2-144">CSV</span><span class="sxs-lookup"><span data-stu-id="906d2-144">CSV</span></span>

<span data-ttu-id="906d2-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="906d2-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="906d2-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="906d2-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="906d2-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="906d2-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="906d2-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="906d2-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="906d2-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="906d2-149">Report Refresh Date</span></span>
- <span data-ttu-id="906d2-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="906d2-150">User Principal Name</span></span>
- <span data-ttu-id="906d2-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="906d2-151">Display Name</span></span>
- <span data-ttu-id="906d2-152">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="906d2-152">User State</span></span>
- <span data-ttu-id="906d2-153">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="906d2-153">State Change Date</span></span>
- <span data-ttu-id="906d2-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="906d2-154">Last Activity Date</span></span>
- <span data-ttu-id="906d2-155">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="906d2-155">Posted Count</span></span>
- <span data-ttu-id="906d2-156">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="906d2-156">Read Count</span></span>
- <span data-ttu-id="906d2-157">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="906d2-157">Liked Count</span></span>
- <span data-ttu-id="906d2-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="906d2-158">Assigned Products</span></span>
- <span data-ttu-id="906d2-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="906d2-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="906d2-160">JSON</span><span class="sxs-lookup"><span data-stu-id="906d2-160">JSON</span></span>

<span data-ttu-id="906d2-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="906d2-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="906d2-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="906d2-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="906d2-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="906d2-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="906d2-164">CSV</span><span class="sxs-lookup"><span data-stu-id="906d2-164">CSV</span></span>

<span data-ttu-id="906d2-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="906d2-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="906d2-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="906d2-166">Request</span></span>

<span data-ttu-id="906d2-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="906d2-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="906d2-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="906d2-168">Response</span></span>

<span data-ttu-id="906d2-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="906d2-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="906d2-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="906d2-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="906d2-171">Basic</span><span class="sxs-lookup"><span data-stu-id="906d2-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="906d2-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="906d2-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="906d2-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="906d2-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="906d2-174">JSON</span><span class="sxs-lookup"><span data-stu-id="906d2-174">JSON</span></span>

<span data-ttu-id="906d2-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="906d2-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="906d2-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="906d2-176">Request</span></span>

<span data-ttu-id="906d2-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="906d2-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="906d2-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="906d2-178">Response</span></span>

<span data-ttu-id="906d2-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="906d2-179">The following is an example of the response.</span></span>

> <span data-ttu-id="906d2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="906d2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="906d2-182">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="906d2-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="906d2-183">Basic</span><span class="sxs-lookup"><span data-stu-id="906d2-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="906d2-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="906d2-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityuserdetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
