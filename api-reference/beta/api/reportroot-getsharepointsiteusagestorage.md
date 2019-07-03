---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ba53c780d8758df8f08d8b2571d713d993c19c55
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446588"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="65b9e-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="65b9e-103">reportRoot: getSharePointSiteUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b9e-104">Obtenha a tendência de armazenamento alocado e consumido durante o período de relatório.</span><span class="sxs-lookup"><span data-stu-id="65b9e-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="65b9e-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="65b9e-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="65b9e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65b9e-106">Permissions</span></span>

<span data-ttu-id="65b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65b9e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65b9e-109">Permission type</span></span>                        | <span data-ttu-id="65b9e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65b9e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65b9e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65b9e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65b9e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65b9e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65b9e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65b9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b9e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65b9e-114">Not supported.</span></span>                           |
| <span data-ttu-id="65b9e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65b9e-115">Application</span></span>                            | <span data-ttu-id="65b9e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65b9e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65b9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65b9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65b9e-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="65b9e-118">Function parameters</span></span>

<span data-ttu-id="65b9e-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="65b9e-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65b9e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="65b9e-120">Parameter</span></span> | <span data-ttu-id="65b9e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="65b9e-121">Type</span></span>   | <span data-ttu-id="65b9e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="65b9e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65b9e-123">ponto</span><span class="sxs-lookup"><span data-stu-id="65b9e-123">period</span></span>    | <span data-ttu-id="65b9e-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65b9e-124">string</span></span> | <span data-ttu-id="65b9e-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="65b9e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65b9e-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="65b9e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65b9e-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="65b9e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65b9e-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65b9e-128">Required.</span></span> |

<span data-ttu-id="65b9e-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65b9e-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="65b9e-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="65b9e-130">The default output type is text/csv.</span></span> <span data-ttu-id="65b9e-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="65b9e-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65b9e-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65b9e-132">Request headers</span></span>

| <span data-ttu-id="65b9e-133">Nome</span><span class="sxs-lookup"><span data-stu-id="65b9e-133">Name</span></span>          | <span data-ttu-id="65b9e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="65b9e-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="65b9e-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="65b9e-135">Authorization</span></span> | <span data-ttu-id="65b9e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65b9e-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="65b9e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b9e-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="65b9e-139">CSV</span><span class="sxs-lookup"><span data-stu-id="65b9e-139">CSV</span></span>

<span data-ttu-id="65b9e-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="65b9e-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65b9e-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="65b9e-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65b9e-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="65b9e-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65b9e-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="65b9e-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65b9e-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="65b9e-144">Report Refresh Date</span></span>
- <span data-ttu-id="65b9e-145">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="65b9e-145">Site Type</span></span>
- <span data-ttu-id="65b9e-146">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="65b9e-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="65b9e-147">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="65b9e-147">Report Date</span></span>
- <span data-ttu-id="65b9e-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="65b9e-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="65b9e-149">JSON</span><span class="sxs-lookup"><span data-stu-id="65b9e-149">JSON</span></span>

<span data-ttu-id="65b9e-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[siteUsageStorage](../resources/siteusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65b9e-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65b9e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65b9e-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="65b9e-152">CSV</span><span class="sxs-lookup"><span data-stu-id="65b9e-152">CSV</span></span>

<span data-ttu-id="65b9e-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="65b9e-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="65b9e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65b9e-154">Request</span></span>

<span data-ttu-id="65b9e-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65b9e-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65b9e-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b9e-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65b9e-157">C#</span><span class="sxs-lookup"><span data-stu-id="65b9e-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65b9e-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="65b9e-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65b9e-159">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="65b9e-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65b9e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b9e-160">Response</span></span>

<span data-ttu-id="65b9e-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65b9e-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="65b9e-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="65b9e-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="65b9e-163">JSON</span><span class="sxs-lookup"><span data-stu-id="65b9e-163">JSON</span></span>

<span data-ttu-id="65b9e-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="65b9e-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="65b9e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65b9e-165">Request</span></span>

<span data-ttu-id="65b9e-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65b9e-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65b9e-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b9e-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65b9e-168">C#</span><span class="sxs-lookup"><span data-stu-id="65b9e-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65b9e-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="65b9e-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65b9e-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="65b9e-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65b9e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b9e-171">Response</span></span>

<span data-ttu-id="65b9e-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65b9e-172">The following is an example of the response.</span></span>

> <span data-ttu-id="65b9e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65b9e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 171835798971, 
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
