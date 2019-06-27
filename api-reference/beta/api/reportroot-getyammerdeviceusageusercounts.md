---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0ddb462cfe21f1a7d2faff1632ca46e77a056c04
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267127"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="4d0e6-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4d0e6-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d0e6-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="4d0e6-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="4d0e6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d0e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d0e6-106">Permissions</span></span>

<span data-ttu-id="4d0e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d0e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d0e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d0e6-109">Permission type</span></span>                        | <span data-ttu-id="4d0e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d0e6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4d0e6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d0e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d0e6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d0e6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4d0e6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d0e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d0e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-114">Not supported.</span></span>                           |
| <span data-ttu-id="4d0e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d0e6-115">Application</span></span>                            | <span data-ttu-id="4d0e6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d0e6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4d0e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d0e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4d0e6-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4d0e6-118">Function parameters</span></span>

<span data-ttu-id="4d0e6-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4d0e6-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4d0e6-120">Parameter</span></span> | <span data-ttu-id="4d0e6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d0e6-121">Type</span></span>   | <span data-ttu-id="4d0e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0e6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4d0e6-123">ponto</span><span class="sxs-lookup"><span data-stu-id="4d0e6-123">period</span></span>    | <span data-ttu-id="4d0e6-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d0e6-124">string</span></span> | <span data-ttu-id="4d0e6-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4d0e6-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4d0e6-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4d0e6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-128">Required.</span></span> |

<span data-ttu-id="4d0e6-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4d0e6-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-130">The default output type is text/csv.</span></span> <span data-ttu-id="4d0e6-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d0e6-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0e6-132">Request headers</span></span>

| <span data-ttu-id="4d0e6-133">Nome</span><span class="sxs-lookup"><span data-stu-id="4d0e6-133">Name</span></span>          | <span data-ttu-id="4d0e6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0e6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4d0e6-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d0e6-135">Authorization</span></span> | <span data-ttu-id="4d0e6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4d0e6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0e6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4d0e6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4d0e6-139">CSV</span></span>

<span data-ttu-id="4d0e6-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4d0e6-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4d0e6-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4d0e6-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4d0e6-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4d0e6-144">Report Refresh Date</span></span>
- <span data-ttu-id="4d0e6-145">Web</span><span class="sxs-lookup"><span data-stu-id="4d0e6-145">Web</span></span>
- <span data-ttu-id="4d0e6-146">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="4d0e6-146">Windows Phone</span></span>
- <span data-ttu-id="4d0e6-147">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="4d0e6-147">Android Phone</span></span>
- <span data-ttu-id="4d0e6-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="4d0e6-148">iPhone</span></span>
- <span data-ttu-id="4d0e6-149">iPad</span><span class="sxs-lookup"><span data-stu-id="4d0e6-149">iPad</span></span>
- <span data-ttu-id="4d0e6-150">Outro</span><span class="sxs-lookup"><span data-stu-id="4d0e6-150">Other</span></span>
- <span data-ttu-id="4d0e6-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4d0e6-151">Report Date</span></span>
- <span data-ttu-id="4d0e6-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4d0e6-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4d0e6-153">JSON</span><span class="sxs-lookup"><span data-stu-id="4d0e6-153">JSON</span></span>

<span data-ttu-id="4d0e6-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d0e6-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d0e6-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4d0e6-156">CSV</span><span class="sxs-lookup"><span data-stu-id="4d0e6-156">CSV</span></span>

<span data-ttu-id="4d0e6-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4d0e6-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0e6-158">Request</span></span>

<span data-ttu-id="4d0e6-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4d0e6-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0e6-160">Response</span></span>

<span data-ttu-id="4d0e6-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d0e6-162">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="4d0e6-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d0e6-163">C#</span><span class="sxs-lookup"><span data-stu-id="4d0e6-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d0e6-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d0e6-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4d0e6-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d0e6-165">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="4d0e6-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4d0e6-167">JSON</span><span class="sxs-lookup"><span data-stu-id="4d0e6-167">JSON</span></span>

<span data-ttu-id="4d0e6-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4d0e6-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0e6-169">Request</span></span>

<span data-ttu-id="4d0e6-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4d0e6-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0e6-171">Response</span></span>

<span data-ttu-id="4d0e6-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-172">The following is an example of the response.</span></span>

> <span data-ttu-id="4d0e6-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d0e6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d0e6-175">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4d0e6-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d0e6-176">C#</span><span class="sxs-lookup"><span data-stu-id="4d0e6-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d0e6-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d0e6-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4d0e6-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d0e6-178">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
