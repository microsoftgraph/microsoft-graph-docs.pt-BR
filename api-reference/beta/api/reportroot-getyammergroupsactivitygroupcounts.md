---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c8fc898bfb9c4a3e7761bb49fea198a95eb527be
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639002"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="1dac1-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="1dac1-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dac1-104">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="1dac1-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="1dac1-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="1dac1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dac1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dac1-106">Permissions</span></span>

<span data-ttu-id="1dac1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dac1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dac1-109">Permission type</span></span>                        | <span data-ttu-id="1dac1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dac1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1dac1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dac1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dac1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dac1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1dac1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dac1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dac1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dac1-114">Not supported.</span></span>                           |
| <span data-ttu-id="1dac1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dac1-115">Application</span></span>                            | <span data-ttu-id="1dac1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dac1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1dac1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dac1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1dac1-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1dac1-118">Function parameters</span></span>

<span data-ttu-id="1dac1-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1dac1-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1dac1-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1dac1-120">Parameter</span></span> | <span data-ttu-id="1dac1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dac1-121">Type</span></span>   | <span data-ttu-id="1dac1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dac1-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1dac1-123">ponto</span><span class="sxs-lookup"><span data-stu-id="1dac1-123">period</span></span>    | <span data-ttu-id="1dac1-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dac1-124">string</span></span> | <span data-ttu-id="1dac1-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1dac1-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1dac1-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1dac1-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1dac1-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1dac1-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1dac1-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dac1-128">Required.</span></span> |

<span data-ttu-id="1dac1-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1dac1-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1dac1-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1dac1-130">The default output type is text/csv.</span></span> <span data-ttu-id="1dac1-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1dac1-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dac1-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dac1-132">Request headers</span></span>

| <span data-ttu-id="1dac1-133">Nome</span><span class="sxs-lookup"><span data-stu-id="1dac1-133">Name</span></span>          | <span data-ttu-id="1dac1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dac1-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1dac1-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dac1-135">Authorization</span></span> | <span data-ttu-id="1dac1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dac1-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1dac1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dac1-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1dac1-139">CSV</span><span class="sxs-lookup"><span data-stu-id="1dac1-139">CSV</span></span>

<span data-ttu-id="1dac1-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1dac1-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1dac1-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1dac1-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1dac1-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1dac1-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1dac1-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1dac1-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1dac1-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1dac1-144">Report Refresh Date</span></span>
- <span data-ttu-id="1dac1-145">Total</span><span class="sxs-lookup"><span data-stu-id="1dac1-145">Total</span></span>
- <span data-ttu-id="1dac1-146">Ativo</span><span class="sxs-lookup"><span data-stu-id="1dac1-146">Active</span></span>
- <span data-ttu-id="1dac1-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1dac1-147">Report Date</span></span>
- <span data-ttu-id="1dac1-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1dac1-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1dac1-149">JSON</span><span class="sxs-lookup"><span data-stu-id="1dac1-149">JSON</span></span>

<span data-ttu-id="1dac1-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dac1-150">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dac1-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dac1-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1dac1-152">CSV</span><span class="sxs-lookup"><span data-stu-id="1dac1-152">CSV</span></span>

<span data-ttu-id="1dac1-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1dac1-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1dac1-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dac1-154">Request</span></span>

<span data-ttu-id="1dac1-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dac1-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1dac1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dac1-156">Response</span></span>

<span data-ttu-id="1dac1-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dac1-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1dac1-158">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1dac1-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1dac1-159">Basic</span><span class="sxs-lookup"><span data-stu-id="1dac1-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dac1-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dac1-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1dac1-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1dac1-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="1dac1-162">JSON</span><span class="sxs-lookup"><span data-stu-id="1dac1-162">JSON</span></span>

<span data-ttu-id="1dac1-163">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1dac1-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1dac1-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dac1-164">Request</span></span>

<span data-ttu-id="1dac1-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dac1-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1dac1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dac1-166">Response</span></span>

<span data-ttu-id="1dac1-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dac1-167">The following is an example of the response.</span></span>

> <span data-ttu-id="1dac1-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dac1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01",
      "total": 50, 
      "active": 41, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1dac1-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1dac1-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1dac1-171">Basic</span><span class="sxs-lookup"><span data-stu-id="1dac1-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dac1-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dac1-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
