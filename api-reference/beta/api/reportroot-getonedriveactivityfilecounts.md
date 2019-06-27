---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e5a7a40e8b1dbbae0031286a89712e7a6729da12
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267316"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="fbcca-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="fbcca-103">reportRoot: getOneDriveActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbcca-104">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fbcca-104">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="fbcca-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="fbcca-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbcca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbcca-106">Permissions</span></span>

<span data-ttu-id="fbcca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fbcca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbcca-109">Permission type</span></span>                        | <span data-ttu-id="fbcca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbcca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fbcca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbcca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbcca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbcca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fbcca-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbcca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbcca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbcca-114">Not supported.</span></span>                           |
| <span data-ttu-id="fbcca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbcca-115">Application</span></span>                            | <span data-ttu-id="fbcca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbcca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fbcca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fbcca-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="fbcca-118">Function parameters</span></span>

<span data-ttu-id="fbcca-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="fbcca-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fbcca-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fbcca-120">Parameter</span></span> | <span data-ttu-id="fbcca-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbcca-121">Type</span></span>   | <span data-ttu-id="fbcca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbcca-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fbcca-123">ponto</span><span class="sxs-lookup"><span data-stu-id="fbcca-123">period</span></span>    | <span data-ttu-id="fbcca-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbcca-124">string</span></span> | <span data-ttu-id="fbcca-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fbcca-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fbcca-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="fbcca-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fbcca-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="fbcca-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fbcca-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbcca-128">Required.</span></span> |

<span data-ttu-id="fbcca-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcca-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fbcca-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="fbcca-130">The default output type is text/csv.</span></span> <span data-ttu-id="fbcca-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="fbcca-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbcca-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcca-132">Request headers</span></span>

| <span data-ttu-id="fbcca-133">Nome</span><span class="sxs-lookup"><span data-stu-id="fbcca-133">Name</span></span>          | <span data-ttu-id="fbcca-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbcca-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fbcca-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbcca-135">Authorization</span></span> | <span data-ttu-id="fbcca-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbcca-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fbcca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbcca-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fbcca-139">CSV</span><span class="sxs-lookup"><span data-stu-id="fbcca-139">CSV</span></span>

<span data-ttu-id="fbcca-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="fbcca-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fbcca-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcca-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fbcca-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fbcca-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fbcca-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="fbcca-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fbcca-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="fbcca-144">Report Refresh Date</span></span>
- <span data-ttu-id="fbcca-145">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="fbcca-145">Viewed Or Edited</span></span>
- <span data-ttu-id="fbcca-146">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="fbcca-146">Synced</span></span>
- <span data-ttu-id="fbcca-147">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="fbcca-147">Shared Internally</span></span>
- <span data-ttu-id="fbcca-148">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="fbcca-148">Shared Externally</span></span>
- <span data-ttu-id="fbcca-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="fbcca-149">Report Date</span></span>
- <span data-ttu-id="fbcca-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="fbcca-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fbcca-151">JSON</span><span class="sxs-lookup"><span data-stu-id="fbcca-151">JSON</span></span>

<span data-ttu-id="fbcca-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[siteActivitySummary](../resources/siteactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcca-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbcca-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbcca-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fbcca-154">CSV</span><span class="sxs-lookup"><span data-stu-id="fbcca-154">CSV</span></span>

<span data-ttu-id="fbcca-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="fbcca-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fbcca-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcca-156">Request</span></span>

<span data-ttu-id="fbcca-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbcca-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="fbcca-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbcca-158">Response</span></span>

<span data-ttu-id="fbcca-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcca-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbcca-160">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="fbcca-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbcca-161">C#</span><span class="sxs-lookup"><span data-stu-id="fbcca-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbcca-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbcca-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fbcca-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fbcca-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="fbcca-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="fbcca-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fbcca-165">JSON</span><span class="sxs-lookup"><span data-stu-id="fbcca-165">JSON</span></span>

<span data-ttu-id="fbcca-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="fbcca-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fbcca-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcca-167">Request</span></span>

<span data-ttu-id="fbcca-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbcca-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="fbcca-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbcca-169">Response</span></span>

<span data-ttu-id="fbcca-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcca-170">The following is an example of the response.</span></span>

> <span data-ttu-id="fbcca-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbcca-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fbcca-173">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fbcca-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fbcca-174">C#</span><span class="sxs-lookup"><span data-stu-id="fbcca-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbcca-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="fbcca-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fbcca-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fbcca-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
