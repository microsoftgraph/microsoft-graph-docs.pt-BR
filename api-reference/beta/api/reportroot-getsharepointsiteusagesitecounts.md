---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 12b025f1d6a5ba9a3f21e8c54f57b8ace18e442a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411407"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="0ac34-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="0ac34-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ac34-105">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="0ac34-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="0ac34-106">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="0ac34-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="0ac34-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="0ac34-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac34-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ac34-108">Permissions</span></span>

<span data-ttu-id="0ac34-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ac34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ac34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ac34-111">Permission type</span></span>                        | <span data-ttu-id="0ac34-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ac34-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0ac34-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ac34-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ac34-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ac34-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0ac34-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ac34-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ac34-116">Not supported.</span></span>                           |
| <span data-ttu-id="0ac34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ac34-117">Application</span></span>                            | <span data-ttu-id="0ac34-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ac34-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0ac34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac34-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0ac34-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0ac34-120">Function parameters</span></span>

<span data-ttu-id="0ac34-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0ac34-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0ac34-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0ac34-122">Parameter</span></span> | <span data-ttu-id="0ac34-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ac34-123">Type</span></span>   | <span data-ttu-id="0ac34-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ac34-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0ac34-125">ponto</span><span class="sxs-lookup"><span data-stu-id="0ac34-125">period</span></span>    | <span data-ttu-id="0ac34-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ac34-126">string</span></span> | <span data-ttu-id="0ac34-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0ac34-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0ac34-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0ac34-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0ac34-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0ac34-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0ac34-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ac34-130">Required.</span></span> |

<span data-ttu-id="0ac34-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac34-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0ac34-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="0ac34-132">The default output type is text/csv.</span></span> <span data-ttu-id="0ac34-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac34-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ac34-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac34-134">Request headers</span></span>

| <span data-ttu-id="0ac34-135">Nome</span><span class="sxs-lookup"><span data-stu-id="0ac34-135">Name</span></span>          | <span data-ttu-id="0ac34-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ac34-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0ac34-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ac34-137">Authorization</span></span> | <span data-ttu-id="0ac34-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ac34-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0ac34-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac34-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0ac34-141">CSV</span><span class="sxs-lookup"><span data-stu-id="0ac34-141">CSV</span></span>

<span data-ttu-id="0ac34-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0ac34-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0ac34-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac34-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0ac34-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0ac34-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0ac34-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0ac34-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0ac34-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0ac34-146">Report Refresh Date</span></span>
- <span data-ttu-id="0ac34-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="0ac34-147">Site Type</span></span>
- <span data-ttu-id="0ac34-148">Total</span><span class="sxs-lookup"><span data-stu-id="0ac34-148">Total</span></span>
- <span data-ttu-id="0ac34-149">Ativo</span><span class="sxs-lookup"><span data-stu-id="0ac34-149">Active</span></span>
- <span data-ttu-id="0ac34-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="0ac34-150">Report Date</span></span>
- <span data-ttu-id="0ac34-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0ac34-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0ac34-152">JSON</span><span class="sxs-lookup"><span data-stu-id="0ac34-152">JSON</span></span>

<span data-ttu-id="0ac34-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac34-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac34-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ac34-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0ac34-155">CSV</span><span class="sxs-lookup"><span data-stu-id="0ac34-155">CSV</span></span>

<span data-ttu-id="0ac34-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="0ac34-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0ac34-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac34-157">Request</span></span>

<span data-ttu-id="0ac34-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ac34-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0ac34-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac34-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ac34-160">C#</span><span class="sxs-lookup"><span data-stu-id="0ac34-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ac34-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ac34-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ac34-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ac34-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ac34-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac34-163">Response</span></span>

<span data-ttu-id="0ac34-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac34-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0ac34-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0ac34-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0ac34-166">JSON</span><span class="sxs-lookup"><span data-stu-id="0ac34-166">JSON</span></span>

<span data-ttu-id="0ac34-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac34-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0ac34-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ac34-168">Request</span></span>

<span data-ttu-id="0ac34-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ac34-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0ac34-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac34-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ac34-171">C#</span><span class="sxs-lookup"><span data-stu-id="0ac34-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ac34-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ac34-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ac34-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ac34-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ac34-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ac34-174">Response</span></span>

<span data-ttu-id="0ac34-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ac34-175">The following is an example of the response.</span></span>

> <span data-ttu-id="0ac34-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ac34-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageSiteCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 47, 
      "active": 15, 
      "reportDate": "2017-09-01", 
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
