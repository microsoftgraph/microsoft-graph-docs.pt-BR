---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5571cd63a136521aed989c3d3222430591f6e7bb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573106"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="4c29d-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="4c29d-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c29d-104">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4c29d-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="4c29d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="4c29d-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c29d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c29d-106">Permissions</span></span>

<span data-ttu-id="4c29d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c29d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c29d-109">Permission type</span></span>                        | <span data-ttu-id="4c29d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c29d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c29d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c29d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c29d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c29d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c29d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c29d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c29d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c29d-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c29d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c29d-115">Application</span></span>                            | <span data-ttu-id="4c29d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c29d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c29d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c29d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4c29d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4c29d-118">Function parameters</span></span>

<span data-ttu-id="4c29d-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4c29d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4c29d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c29d-120">Parameter</span></span> | <span data-ttu-id="4c29d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c29d-121">Type</span></span>   | <span data-ttu-id="4c29d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c29d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c29d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="4c29d-123">period</span></span>    | <span data-ttu-id="4c29d-124">string</span><span class="sxs-lookup"><span data-stu-id="4c29d-124">string</span></span> | <span data-ttu-id="4c29d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c29d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c29d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4c29d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c29d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c29d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4c29d-128">data</span><span class="sxs-lookup"><span data-stu-id="4c29d-128">date</span></span>      | <span data-ttu-id="4c29d-129">Data</span><span class="sxs-lookup"><span data-stu-id="4c29d-129">Date</span></span>   | <span data-ttu-id="4c29d-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="4c29d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4c29d-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="4c29d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4c29d-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="4c29d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4c29d-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="4c29d-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4c29d-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="4c29d-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c29d-135">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="4c29d-135">The default output type is text/csv.</span></span> <span data-ttu-id="4c29d-136">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="4c29d-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c29d-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c29d-137">Request headers</span></span>

| <span data-ttu-id="4c29d-138">Nome</span><span class="sxs-lookup"><span data-stu-id="4c29d-138">Name</span></span>          | <span data-ttu-id="4c29d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c29d-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c29d-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c29d-140">Authorization</span></span> | <span data-ttu-id="4c29d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c29d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c29d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c29d-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c29d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4c29d-144">CSV</span></span>

<span data-ttu-id="4c29d-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4c29d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c29d-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4c29d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c29d-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c29d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c29d-148">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="4c29d-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="4c29d-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4c29d-149">Report Refresh Date</span></span>
- <span data-ttu-id="4c29d-150">Id do site</span><span class="sxs-lookup"><span data-stu-id="4c29d-150">Site Id</span></span>
- <span data-ttu-id="4c29d-151">URL do site</span><span class="sxs-lookup"><span data-stu-id="4c29d-151">Site URL</span></span>
- <span data-ttu-id="4c29d-152">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="4c29d-152">Owner Display Name</span></span>
- <span data-ttu-id="4c29d-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="4c29d-153">Is Deleted</span></span>
- <span data-ttu-id="4c29d-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="4c29d-154">Last Activity Date</span></span>
- <span data-ttu-id="4c29d-155">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="4c29d-155">File Count</span></span>
- <span data-ttu-id="4c29d-156">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="4c29d-156">Active File Count</span></span>
- <span data-ttu-id="4c29d-157">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="4c29d-157">Page View Count</span></span>
- <span data-ttu-id="4c29d-158">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="4c29d-158">Visited Page Count</span></span>
- <span data-ttu-id="4c29d-159">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="4c29d-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="4c29d-160">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="4c29d-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="4c29d-161">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="4c29d-161">Root Web Template</span></span>
- <span data-ttu-id="4c29d-162">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4c29d-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4c29d-163">JSON</span><span class="sxs-lookup"><span data-stu-id="4c29d-163">JSON</span></span>

<span data-ttu-id="4c29d-164">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c29d-164">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="4c29d-165">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="4c29d-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4c29d-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c29d-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c29d-167">CSV</span><span class="sxs-lookup"><span data-stu-id="4c29d-167">CSV</span></span>

<span data-ttu-id="4c29d-168">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="4c29d-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c29d-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c29d-169">Request</span></span>

<span data-ttu-id="4c29d-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c29d-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4c29d-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c29d-171">Response</span></span>

<span data-ttu-id="4c29d-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c29d-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c29d-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4c29d-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```

### <a name="json"></a><span data-ttu-id="4c29d-174">JSON</span><span class="sxs-lookup"><span data-stu-id="4c29d-174">JSON</span></span>

<span data-ttu-id="4c29d-175">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="4c29d-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c29d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c29d-176">Request</span></span>

<span data-ttu-id="4c29d-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c29d-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4c29d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c29d-178">Response</span></span>

<span data-ttu-id="4c29d-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c29d-179">The following is an example of the response.</span></span>

> <span data-ttu-id="4c29d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c29d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagedetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
