---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: efe032dcf29ae316487fbfacf3a38cad7373b6f7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265125"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="d04fa-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d04fa-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d04fa-104">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="d04fa-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="d04fa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d04fa-105">Permissions</span></span>

<span data-ttu-id="d04fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d04fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d04fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d04fa-108">Permission type</span></span>                        | <span data-ttu-id="d04fa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d04fa-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d04fa-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d04fa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d04fa-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d04fa-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d04fa-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d04fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d04fa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d04fa-113">Not supported.</span></span>                           |
| <span data-ttu-id="d04fa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d04fa-114">Application</span></span>                            | <span data-ttu-id="d04fa-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d04fa-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d04fa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d04fa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="d04fa-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d04fa-117">Function parameters</span></span>

<span data-ttu-id="d04fa-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d04fa-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d04fa-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d04fa-119">Parameter</span></span> | <span data-ttu-id="d04fa-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d04fa-120">Type</span></span>   | <span data-ttu-id="d04fa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d04fa-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d04fa-122">ponto</span><span class="sxs-lookup"><span data-stu-id="d04fa-122">period</span></span>    | <span data-ttu-id="d04fa-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d04fa-123">string</span></span> | <span data-ttu-id="d04fa-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d04fa-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d04fa-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d04fa-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d04fa-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d04fa-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d04fa-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d04fa-127">Required.</span></span> |

<span data-ttu-id="d04fa-128">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d04fa-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d04fa-129">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d04fa-129">The default output type is text/csv.</span></span> <span data-ttu-id="d04fa-130">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d04fa-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d04fa-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d04fa-131">Request headers</span></span>

| <span data-ttu-id="d04fa-132">Nome</span><span class="sxs-lookup"><span data-stu-id="d04fa-132">Name</span></span>          | <span data-ttu-id="d04fa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d04fa-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d04fa-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="d04fa-134">Authorization</span></span> | <span data-ttu-id="d04fa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d04fa-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d04fa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d04fa-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d04fa-138">CSV</span><span class="sxs-lookup"><span data-stu-id="d04fa-138">CSV</span></span>

<span data-ttu-id="d04fa-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d04fa-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d04fa-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d04fa-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d04fa-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d04fa-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d04fa-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d04fa-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d04fa-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d04fa-143">Report Refresh Date</span></span>
- <span data-ttu-id="d04fa-144">Web</span><span class="sxs-lookup"><span data-stu-id="d04fa-144">Web</span></span>
- <span data-ttu-id="d04fa-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d04fa-145">Windows Phone</span></span>
- <span data-ttu-id="d04fa-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d04fa-146">Android Phone</span></span>
- <span data-ttu-id="d04fa-147">iOS</span><span class="sxs-lookup"><span data-stu-id="d04fa-147">iOS</span></span>
- <span data-ttu-id="d04fa-148">Mac</span><span class="sxs-lookup"><span data-stu-id="d04fa-148">Mac</span></span>
- <span data-ttu-id="d04fa-149">Windows</span><span class="sxs-lookup"><span data-stu-id="d04fa-149">Windows</span></span>
- <span data-ttu-id="d04fa-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d04fa-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d04fa-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d04fa-151">JSON</span></span>

<span data-ttu-id="d04fa-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d04fa-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d04fa-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d04fa-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d04fa-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d04fa-154">CSV</span></span>

<span data-ttu-id="d04fa-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d04fa-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d04fa-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d04fa-156">Request</span></span>

<span data-ttu-id="d04fa-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d04fa-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d04fa-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d04fa-158">Response</span></span>

<span data-ttu-id="d04fa-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d04fa-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d04fa-160">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="d04fa-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d04fa-161">C#</span><span class="sxs-lookup"><span data-stu-id="d04fa-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d04fa-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="d04fa-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d04fa-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d04fa-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d04fa-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d04fa-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="d04fa-165">JSON</span><span class="sxs-lookup"><span data-stu-id="d04fa-165">JSON</span></span>

<span data-ttu-id="d04fa-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d04fa-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d04fa-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d04fa-167">Request</span></span>

<span data-ttu-id="d04fa-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d04fa-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d04fa-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d04fa-169">Response</span></span>

<span data-ttu-id="d04fa-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d04fa-170">The following is an example of the response.</span></span>

> <span data-ttu-id="d04fa-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d04fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d04fa-173">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d04fa-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d04fa-174">C#</span><span class="sxs-lookup"><span data-stu-id="d04fa-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d04fa-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="d04fa-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d04fa-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d04fa-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsdeviceusagedistributionusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
