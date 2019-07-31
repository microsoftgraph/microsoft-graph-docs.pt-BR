---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 32ac301fc74d974c5520e4d3f0c526c693777be6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983191"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="c5ade-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c5ade-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5ade-104">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="c5ade-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="c5ade-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5ade-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5ade-106">Permissions</span></span>

<span data-ttu-id="c5ade-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5ade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5ade-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5ade-109">Permission type</span></span>                        | <span data-ttu-id="c5ade-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5ade-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5ade-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5ade-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5ade-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5ade-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5ade-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5ade-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5ade-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5ade-114">Not supported.</span></span>                           |
| <span data-ttu-id="c5ade-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5ade-115">Application</span></span>                            | <span data-ttu-id="c5ade-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5ade-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5ade-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5ade-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c5ade-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c5ade-118">Function parameters</span></span>

<span data-ttu-id="c5ade-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c5ade-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c5ade-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c5ade-120">Parameter</span></span> | <span data-ttu-id="c5ade-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5ade-121">Type</span></span>   | <span data-ttu-id="c5ade-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5ade-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c5ade-123">ponto</span><span class="sxs-lookup"><span data-stu-id="c5ade-123">period</span></span>    | <span data-ttu-id="c5ade-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5ade-124">string</span></span> | <span data-ttu-id="c5ade-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c5ade-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c5ade-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c5ade-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c5ade-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c5ade-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c5ade-128">data</span><span class="sxs-lookup"><span data-stu-id="c5ade-128">date</span></span>      | <span data-ttu-id="c5ade-129">Data</span><span class="sxs-lookup"><span data-stu-id="c5ade-129">Date</span></span>   | <span data-ttu-id="c5ade-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="c5ade-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c5ade-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="c5ade-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c5ade-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="c5ade-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c5ade-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="c5ade-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c5ade-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c5ade-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="c5ade-135">The default output type is text/csv.</span></span> <span data-ttu-id="c5ade-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c5ade-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5ade-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5ade-137">Request headers</span></span>

| <span data-ttu-id="c5ade-138">Nome</span><span class="sxs-lookup"><span data-stu-id="c5ade-138">Name</span></span>          | <span data-ttu-id="c5ade-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5ade-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c5ade-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5ade-140">Authorization</span></span> | <span data-ttu-id="c5ade-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5ade-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5ade-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5ade-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c5ade-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c5ade-144">CSV</span></span>

<span data-ttu-id="c5ade-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c5ade-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5ade-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5ade-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c5ade-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5ade-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c5ade-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5ade-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c5ade-149">Report Refresh Date</span></span>
- <span data-ttu-id="c5ade-150">URL do site</span><span class="sxs-lookup"><span data-stu-id="c5ade-150">Site URL</span></span>
- <span data-ttu-id="c5ade-151">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="c5ade-151">Owner Display Name</span></span>
- <span data-ttu-id="c5ade-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="c5ade-152">Is Deleted</span></span>
- <span data-ttu-id="c5ade-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="c5ade-153">Last Activity Date</span></span>
- <span data-ttu-id="c5ade-154">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="c5ade-154">File Count</span></span>
- <span data-ttu-id="c5ade-155">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="c5ade-155">Active File Count</span></span>
- <span data-ttu-id="c5ade-156">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="c5ade-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="c5ade-157">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="c5ade-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="c5ade-158">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="c5ade-158">Owner Principal Name</span></span>
- <span data-ttu-id="c5ade-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c5ade-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c5ade-160">JSON</span><span class="sxs-lookup"><span data-stu-id="c5ade-160">JSON</span></span>

<span data-ttu-id="c5ade-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-161">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c5ade-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="c5ade-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c5ade-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5ade-163">Example</span></span>

<span data-ttu-id="c5ade-164">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="c5ade-164">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="c5ade-165">CSV</span><span class="sxs-lookup"><span data-stu-id="c5ade-165">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="c5ade-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5ade-166">Request</span></span>

<span data-ttu-id="c5ade-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5ade-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c5ade-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5ade-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5ade-169">C#</span><span class="sxs-lookup"><span data-stu-id="c5ade-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5ade-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5ade-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5ade-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c5ade-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5ade-172">Java</span><span class="sxs-lookup"><span data-stu-id="c5ade-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageaccountdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5ade-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5ade-173">Response</span></span>

<span data-ttu-id="c5ade-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c5ade-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c5ade-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="c5ade-176">JSON</span><span class="sxs-lookup"><span data-stu-id="c5ade-176">JSON</span></span>

<span data-ttu-id="c5ade-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="c5ade-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c5ade-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5ade-178">Request</span></span>

<span data-ttu-id="c5ade-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5ade-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c5ade-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5ade-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5ade-181">C#</span><span class="sxs-lookup"><span data-stu-id="c5ade-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5ade-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5ade-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5ade-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c5ade-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5ade-184">Java</span><span class="sxs-lookup"><span data-stu-id="c5ade-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageaccountdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5ade-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5ade-185">Response</span></span>

<span data-ttu-id="c5ade-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5ade-186">The following is an example of the response.</span></span>

> <span data-ttu-id="c5ade-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5ade-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
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
