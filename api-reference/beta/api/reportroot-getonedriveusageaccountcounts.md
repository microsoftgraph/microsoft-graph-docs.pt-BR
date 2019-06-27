---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 14025632d10487abb1e0a9710c2a940e3555f4b8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265349"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="bc14c-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="bc14c-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc14c-105">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="bc14c-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="bc14c-106">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="bc14c-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="bc14c-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="bc14c-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc14c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc14c-108">Permissions</span></span>

<span data-ttu-id="bc14c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc14c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc14c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc14c-111">Permission type</span></span>                        | <span data-ttu-id="bc14c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc14c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bc14c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc14c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc14c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc14c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bc14c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc14c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc14c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc14c-116">Not supported.</span></span>                           |
| <span data-ttu-id="bc14c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc14c-117">Application</span></span>                            | <span data-ttu-id="bc14c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc14c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bc14c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc14c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bc14c-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bc14c-120">Function parameters</span></span>

<span data-ttu-id="bc14c-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bc14c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bc14c-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bc14c-122">Parameter</span></span> | <span data-ttu-id="bc14c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc14c-123">Type</span></span>   | <span data-ttu-id="bc14c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc14c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bc14c-125">ponto</span><span class="sxs-lookup"><span data-stu-id="bc14c-125">period</span></span>    | <span data-ttu-id="bc14c-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14c-126">string</span></span> | <span data-ttu-id="bc14c-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bc14c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bc14c-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bc14c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bc14c-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bc14c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bc14c-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc14c-130">Required.</span></span> |

<span data-ttu-id="bc14c-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bc14c-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bc14c-132">The default output type is text/csv.</span></span> <span data-ttu-id="bc14c-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bc14c-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc14c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-134">Request headers</span></span>

| <span data-ttu-id="bc14c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="bc14c-135">Name</span></span>          | <span data-ttu-id="bc14c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc14c-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bc14c-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc14c-137">Authorization</span></span> | <span data-ttu-id="bc14c-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc14c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bc14c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14c-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bc14c-141">CSV</span><span class="sxs-lookup"><span data-stu-id="bc14c-141">CSV</span></span>

<span data-ttu-id="bc14c-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bc14c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bc14c-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bc14c-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bc14c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bc14c-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bc14c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bc14c-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bc14c-146">Report Refresh Date</span></span>
- <span data-ttu-id="bc14c-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="bc14c-147">Site Type</span></span>
- <span data-ttu-id="bc14c-148">Total</span><span class="sxs-lookup"><span data-stu-id="bc14c-148">Total</span></span>
- <span data-ttu-id="bc14c-149">Ativo</span><span class="sxs-lookup"><span data-stu-id="bc14c-149">Active</span></span>
- <span data-ttu-id="bc14c-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="bc14c-150">Report Date</span></span>
- <span data-ttu-id="bc14c-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bc14c-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bc14c-152">JSON</span><span class="sxs-lookup"><span data-stu-id="bc14c-152">JSON</span></span>

<span data-ttu-id="bc14c-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc14c-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc14c-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bc14c-155">CSV</span><span class="sxs-lookup"><span data-stu-id="bc14c-155">CSV</span></span>

<span data-ttu-id="bc14c-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bc14c-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bc14c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-157">Request</span></span>

<span data-ttu-id="bc14c-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc14c-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bc14c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14c-159">Response</span></span>

<span data-ttu-id="bc14c-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc14c-161">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="bc14c-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc14c-162">C#</span><span class="sxs-lookup"><span data-stu-id="bc14c-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc14c-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc14c-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bc14c-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bc14c-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bc14c-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bc14c-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="bc14c-166">JSON</span><span class="sxs-lookup"><span data-stu-id="bc14c-166">JSON</span></span>

<span data-ttu-id="bc14c-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bc14c-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bc14c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-168">Request</span></span>

<span data-ttu-id="bc14c-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc14c-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bc14c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14c-170">Response</span></span>

<span data-ttu-id="bc14c-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-171">The following is an example of the response.</span></span>

> <span data-ttu-id="bc14c-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc14c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc14c-174">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bc14c-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc14c-175">C#</span><span class="sxs-lookup"><span data-stu-id="bc14c-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc14c-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc14c-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bc14c-177">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bc14c-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountcounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
