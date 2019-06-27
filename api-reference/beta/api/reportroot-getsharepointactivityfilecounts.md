---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e28cc85dfb20f7255a792121208129e4a571834d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265286"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="bd53d-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="bd53d-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd53d-104">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bd53d-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="bd53d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="bd53d-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd53d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd53d-106">Permissions</span></span>

<span data-ttu-id="bd53d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd53d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd53d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd53d-109">Permission type</span></span>                        | <span data-ttu-id="bd53d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd53d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bd53d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd53d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd53d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd53d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bd53d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd53d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd53d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd53d-114">Not supported.</span></span>                           |
| <span data-ttu-id="bd53d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd53d-115">Application</span></span>                            | <span data-ttu-id="bd53d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd53d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bd53d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd53d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bd53d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bd53d-118">Function parameters</span></span>

<span data-ttu-id="bd53d-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bd53d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bd53d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bd53d-120">Parameter</span></span> | <span data-ttu-id="bd53d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd53d-121">Type</span></span>   | <span data-ttu-id="bd53d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd53d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bd53d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="bd53d-123">period</span></span>    | <span data-ttu-id="bd53d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd53d-124">string</span></span> | <span data-ttu-id="bd53d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bd53d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bd53d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bd53d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bd53d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bd53d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bd53d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd53d-128">Required.</span></span> |

<span data-ttu-id="bd53d-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd53d-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bd53d-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bd53d-130">The default output type is text/csv.</span></span> <span data-ttu-id="bd53d-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bd53d-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd53d-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd53d-132">Request headers</span></span>

| <span data-ttu-id="bd53d-133">Nome</span><span class="sxs-lookup"><span data-stu-id="bd53d-133">Name</span></span>          | <span data-ttu-id="bd53d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd53d-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bd53d-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd53d-135">Authorization</span></span> | <span data-ttu-id="bd53d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd53d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bd53d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd53d-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bd53d-139">CSV</span><span class="sxs-lookup"><span data-stu-id="bd53d-139">CSV</span></span>

<span data-ttu-id="bd53d-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bd53d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bd53d-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bd53d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bd53d-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bd53d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bd53d-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bd53d-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bd53d-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bd53d-144">Report Refresh Date</span></span>
- <span data-ttu-id="bd53d-145">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="bd53d-145">Viewed Or Edited</span></span>
- <span data-ttu-id="bd53d-146">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="bd53d-146">Synced</span></span>
- <span data-ttu-id="bd53d-147">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="bd53d-147">Shared Internally</span></span>
- <span data-ttu-id="bd53d-148">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="bd53d-148">Shared Externally</span></span>
- <span data-ttu-id="bd53d-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="bd53d-149">Report Date</span></span>
- <span data-ttu-id="bd53d-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bd53d-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bd53d-151">JSON</span><span class="sxs-lookup"><span data-stu-id="bd53d-151">JSON</span></span>

<span data-ttu-id="bd53d-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[siteActivitySummary](../resources/siteactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd53d-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd53d-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd53d-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bd53d-154">CSV</span><span class="sxs-lookup"><span data-stu-id="bd53d-154">CSV</span></span>

<span data-ttu-id="bd53d-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bd53d-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bd53d-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd53d-156">Request</span></span>

<span data-ttu-id="bd53d-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd53d-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bd53d-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd53d-158">Response</span></span>

<span data-ttu-id="bd53d-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd53d-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd53d-160">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="bd53d-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd53d-161">C#</span><span class="sxs-lookup"><span data-stu-id="bd53d-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd53d-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd53d-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bd53d-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bd53d-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointactivityfilecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bd53d-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bd53d-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="bd53d-165">JSON</span><span class="sxs-lookup"><span data-stu-id="bd53d-165">JSON</span></span>

<span data-ttu-id="bd53d-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bd53d-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bd53d-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd53d-167">Request</span></span>

<span data-ttu-id="bd53d-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd53d-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bd53d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd53d-169">Response</span></span>

<span data-ttu-id="bd53d-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd53d-170">The following is an example of the response.</span></span>

> <span data-ttu-id="bd53d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd53d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bd53d-173">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bd53d-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bd53d-174">C#</span><span class="sxs-lookup"><span data-stu-id="bd53d-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd53d-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd53d-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bd53d-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bd53d-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
