---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cbe6929f51ef52b1e33f7f81a0263a9a90c4763d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872683"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="a22ec-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a22ec-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a22ec-104">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a22ec-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="a22ec-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="a22ec-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="a22ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a22ec-106">Permissions</span></span>

<span data-ttu-id="a22ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a22ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a22ec-109">Permission type</span></span>                        | <span data-ttu-id="a22ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a22ec-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a22ec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a22ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a22ec-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22ec-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a22ec-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a22ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a22ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a22ec-114">Not supported.</span></span>                           |
| <span data-ttu-id="a22ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a22ec-115">Application</span></span>                            | <span data-ttu-id="a22ec-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22ec-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a22ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a22ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a22ec-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a22ec-118">Function parameters</span></span>

<span data-ttu-id="a22ec-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a22ec-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a22ec-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a22ec-120">Parameter</span></span> | <span data-ttu-id="a22ec-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a22ec-121">Type</span></span>   | <span data-ttu-id="a22ec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a22ec-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a22ec-123">ponto</span><span class="sxs-lookup"><span data-stu-id="a22ec-123">period</span></span>    | <span data-ttu-id="a22ec-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a22ec-124">string</span></span> | <span data-ttu-id="a22ec-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a22ec-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a22ec-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a22ec-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a22ec-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a22ec-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a22ec-128">data</span><span class="sxs-lookup"><span data-stu-id="a22ec-128">date</span></span>      | <span data-ttu-id="a22ec-129">Data</span><span class="sxs-lookup"><span data-stu-id="a22ec-129">Date</span></span>   | <span data-ttu-id="a22ec-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="a22ec-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a22ec-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a22ec-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a22ec-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="a22ec-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a22ec-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="a22ec-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a22ec-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="a22ec-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a22ec-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="a22ec-135">The default output type is text/csv.</span></span> <span data-ttu-id="a22ec-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a22ec-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a22ec-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a22ec-137">Request headers</span></span>

| <span data-ttu-id="a22ec-138">Nome</span><span class="sxs-lookup"><span data-stu-id="a22ec-138">Name</span></span>          | <span data-ttu-id="a22ec-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a22ec-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a22ec-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="a22ec-140">Authorization</span></span> | <span data-ttu-id="a22ec-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a22ec-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a22ec-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22ec-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a22ec-144">CSV</span><span class="sxs-lookup"><span data-stu-id="a22ec-144">CSV</span></span>

<span data-ttu-id="a22ec-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a22ec-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a22ec-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a22ec-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a22ec-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a22ec-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a22ec-148">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="a22ec-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="a22ec-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a22ec-149">Report Refresh Date</span></span>
- <span data-ttu-id="a22ec-150">ID de site</span><span class="sxs-lookup"><span data-stu-id="a22ec-150">Site Id</span></span>
- <span data-ttu-id="a22ec-151">URL do site</span><span class="sxs-lookup"><span data-stu-id="a22ec-151">Site URL</span></span>
- <span data-ttu-id="a22ec-152">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="a22ec-152">Owner Display Name</span></span>
- <span data-ttu-id="a22ec-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="a22ec-153">Is Deleted</span></span>
- <span data-ttu-id="a22ec-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="a22ec-154">Last Activity Date</span></span>
- <span data-ttu-id="a22ec-155">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="a22ec-155">File Count</span></span>
- <span data-ttu-id="a22ec-156">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="a22ec-156">Active File Count</span></span>
- <span data-ttu-id="a22ec-157">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="a22ec-157">Page View Count</span></span>
- <span data-ttu-id="a22ec-158">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="a22ec-158">Visited Page Count</span></span>
- <span data-ttu-id="a22ec-159">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a22ec-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="a22ec-160">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a22ec-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="a22ec-161">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="a22ec-161">Root Web Template</span></span>
- <span data-ttu-id="a22ec-162">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="a22ec-162">Owner Principal Name</span></span>
- <span data-ttu-id="a22ec-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a22ec-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a22ec-164">JSON</span><span class="sxs-lookup"><span data-stu-id="a22ec-164">JSON</span></span>

<span data-ttu-id="a22ec-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a22ec-165">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="a22ec-166">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="a22ec-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a22ec-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a22ec-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a22ec-168">CSV</span><span class="sxs-lookup"><span data-stu-id="a22ec-168">CSV</span></span>

<span data-ttu-id="a22ec-169">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="a22ec-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a22ec-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a22ec-170">Request</span></span>

<span data-ttu-id="a22ec-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a22ec-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a22ec-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a22ec-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a22ec-173">C#</span><span class="sxs-lookup"><span data-stu-id="a22ec-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a22ec-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="a22ec-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a22ec-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a22ec-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a22ec-176">Java</span><span class="sxs-lookup"><span data-stu-id="a22ec-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a22ec-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22ec-177">Response</span></span>

<span data-ttu-id="a22ec-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a22ec-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a22ec-179">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a22ec-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="a22ec-180">JSON</span><span class="sxs-lookup"><span data-stu-id="a22ec-180">JSON</span></span>

<span data-ttu-id="a22ec-181">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="a22ec-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a22ec-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a22ec-182">Request</span></span>

<span data-ttu-id="a22ec-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a22ec-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a22ec-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="a22ec-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a22ec-185">C#</span><span class="sxs-lookup"><span data-stu-id="a22ec-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a22ec-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="a22ec-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a22ec-187">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a22ec-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a22ec-188">Java</span><span class="sxs-lookup"><span data-stu-id="a22ec-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a22ec-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a22ec-189">Response</span></span>

<span data-ttu-id="a22ec-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a22ec-190">The following is an example of the response.</span></span>

> <span data-ttu-id="a22ec-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a22ec-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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
