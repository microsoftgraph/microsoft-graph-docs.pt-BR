---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos. Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d0703586005f229f1bb905507e702d8bec55f97a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446728"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="d53aa-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="d53aa-104">reportRoot: getOneDriveUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d53aa-105">Obtenha o número total de arquivos em todos os sites e quantos são arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="d53aa-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="d53aa-106">Um arquivo é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d53aa-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="d53aa-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="d53aa-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="d53aa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d53aa-108">Permissions</span></span>

<span data-ttu-id="d53aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d53aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d53aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d53aa-111">Permission type</span></span>                        | <span data-ttu-id="d53aa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d53aa-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d53aa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d53aa-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d53aa-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d53aa-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d53aa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d53aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d53aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d53aa-116">Not supported.</span></span>                           |
| <span data-ttu-id="d53aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d53aa-117">Application</span></span>                            | <span data-ttu-id="d53aa-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d53aa-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d53aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d53aa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d53aa-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d53aa-120">Function parameters</span></span>

<span data-ttu-id="d53aa-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d53aa-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d53aa-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d53aa-122">Parameter</span></span> | <span data-ttu-id="d53aa-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d53aa-123">Type</span></span>   | <span data-ttu-id="d53aa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53aa-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d53aa-125">ponto</span><span class="sxs-lookup"><span data-stu-id="d53aa-125">period</span></span>    | <span data-ttu-id="d53aa-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d53aa-126">string</span></span> | <span data-ttu-id="d53aa-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d53aa-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d53aa-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d53aa-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d53aa-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d53aa-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d53aa-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d53aa-130">Required.</span></span> |

<span data-ttu-id="d53aa-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d53aa-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d53aa-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d53aa-132">The default output type is text/csv.</span></span> <span data-ttu-id="d53aa-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d53aa-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d53aa-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d53aa-134">Request headers</span></span>

| <span data-ttu-id="d53aa-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d53aa-135">Name</span></span>          | <span data-ttu-id="d53aa-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53aa-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d53aa-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d53aa-137">Authorization</span></span> | <span data-ttu-id="d53aa-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d53aa-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d53aa-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d53aa-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d53aa-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d53aa-141">CSV</span></span>

<span data-ttu-id="d53aa-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d53aa-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d53aa-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d53aa-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d53aa-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d53aa-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d53aa-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d53aa-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d53aa-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d53aa-146">Report Refresh Date</span></span>
- <span data-ttu-id="d53aa-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="d53aa-147">Site Type</span></span>
- <span data-ttu-id="d53aa-148">Total</span><span class="sxs-lookup"><span data-stu-id="d53aa-148">Total</span></span>
- <span data-ttu-id="d53aa-149">Ativo</span><span class="sxs-lookup"><span data-stu-id="d53aa-149">Active</span></span>
- <span data-ttu-id="d53aa-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d53aa-150">Report Date</span></span>
- <span data-ttu-id="d53aa-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d53aa-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d53aa-152">JSON</span><span class="sxs-lookup"><span data-stu-id="d53aa-152">JSON</span></span>

<span data-ttu-id="d53aa-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d53aa-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d53aa-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d53aa-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d53aa-155">CSV</span><span class="sxs-lookup"><span data-stu-id="d53aa-155">CSV</span></span>

<span data-ttu-id="d53aa-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d53aa-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d53aa-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d53aa-157">Request</span></span>

<span data-ttu-id="d53aa-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d53aa-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d53aa-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="d53aa-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d53aa-160">C#</span><span class="sxs-lookup"><span data-stu-id="d53aa-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d53aa-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="d53aa-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d53aa-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d53aa-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d53aa-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d53aa-163">Response</span></span>

<span data-ttu-id="d53aa-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d53aa-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d53aa-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d53aa-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d53aa-166">JSON</span><span class="sxs-lookup"><span data-stu-id="d53aa-166">JSON</span></span>

<span data-ttu-id="d53aa-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d53aa-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d53aa-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d53aa-168">Request</span></span>

<span data-ttu-id="d53aa-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d53aa-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d53aa-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="d53aa-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d53aa-171">C#</span><span class="sxs-lookup"><span data-stu-id="d53aa-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d53aa-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="d53aa-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d53aa-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d53aa-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d53aa-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="d53aa-174">Response</span></span>

<span data-ttu-id="d53aa-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d53aa-175">The following is an example of the response.</span></span>

> <span data-ttu-id="d53aa-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d53aa-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 297960, 
      "active": 4679, 
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
