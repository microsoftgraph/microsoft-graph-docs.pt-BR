---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ed88ec08937aca01ca05a6334a2fe3f08fe65e4e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724838"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="b8e69-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b8e69-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8e69-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8e69-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="b8e69-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="b8e69-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8e69-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8e69-106">Permissions</span></span>

<span data-ttu-id="b8e69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8e69-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8e69-109">Permission type</span></span>                        | <span data-ttu-id="b8e69-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8e69-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b8e69-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8e69-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8e69-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8e69-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b8e69-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8e69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8e69-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8e69-114">Not supported.</span></span>                           |
| <span data-ttu-id="b8e69-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8e69-115">Application</span></span>                            | <span data-ttu-id="b8e69-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8e69-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b8e69-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e69-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b8e69-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b8e69-118">Function parameters</span></span>

<span data-ttu-id="b8e69-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b8e69-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b8e69-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8e69-120">Parameter</span></span> | <span data-ttu-id="b8e69-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8e69-121">Type</span></span>   | <span data-ttu-id="b8e69-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e69-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b8e69-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b8e69-123">period</span></span>    | <span data-ttu-id="b8e69-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8e69-124">string</span></span> | <span data-ttu-id="b8e69-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b8e69-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b8e69-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b8e69-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b8e69-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b8e69-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b8e69-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8e69-128">Required.</span></span> |

<span data-ttu-id="b8e69-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e69-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b8e69-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="b8e69-130">The default output type is text/csv.</span></span> <span data-ttu-id="b8e69-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b8e69-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8e69-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e69-132">Request headers</span></span>

| <span data-ttu-id="b8e69-133">Nome</span><span class="sxs-lookup"><span data-stu-id="b8e69-133">Name</span></span>          | <span data-ttu-id="b8e69-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e69-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b8e69-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8e69-135">Authorization</span></span> | <span data-ttu-id="b8e69-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8e69-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b8e69-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e69-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b8e69-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b8e69-139">CSV</span></span>

<span data-ttu-id="b8e69-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b8e69-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b8e69-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e69-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b8e69-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b8e69-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b8e69-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b8e69-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b8e69-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b8e69-144">Report Refresh Date</span></span>
- <span data-ttu-id="b8e69-145">Web</span><span class="sxs-lookup"><span data-stu-id="b8e69-145">Web</span></span>
- <span data-ttu-id="b8e69-146">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b8e69-146">Windows Phone</span></span>
- <span data-ttu-id="b8e69-147">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="b8e69-147">Android Phone</span></span>
- <span data-ttu-id="b8e69-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="b8e69-148">iPhone</span></span>
- <span data-ttu-id="b8e69-149">iPad</span><span class="sxs-lookup"><span data-stu-id="b8e69-149">iPad</span></span>
- <span data-ttu-id="b8e69-150">Outro</span><span class="sxs-lookup"><span data-stu-id="b8e69-150">Other</span></span>
- <span data-ttu-id="b8e69-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b8e69-151">Report Date</span></span>
- <span data-ttu-id="b8e69-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b8e69-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b8e69-153">JSON</span><span class="sxs-lookup"><span data-stu-id="b8e69-153">JSON</span></span>

<span data-ttu-id="b8e69-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e69-154">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e69-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8e69-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b8e69-156">CSV</span><span class="sxs-lookup"><span data-stu-id="b8e69-156">CSV</span></span>

<span data-ttu-id="b8e69-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="b8e69-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b8e69-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e69-158">Request</span></span>

<span data-ttu-id="b8e69-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8e69-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b8e69-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e69-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8e69-161">C#</span><span class="sxs-lookup"><span data-stu-id="b8e69-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8e69-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8e69-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8e69-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8e69-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8e69-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e69-164">Response</span></span>

<span data-ttu-id="b8e69-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e69-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b8e69-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b8e69-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b8e69-167">JSON</span><span class="sxs-lookup"><span data-stu-id="b8e69-167">JSON</span></span>

<span data-ttu-id="b8e69-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="b8e69-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b8e69-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8e69-169">Request</span></span>

<span data-ttu-id="b8e69-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8e69-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b8e69-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8e69-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8e69-172">C#</span><span class="sxs-lookup"><span data-stu-id="b8e69-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8e69-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8e69-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8e69-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8e69-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8e69-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8e69-175">Response</span></span>

<span data-ttu-id="b8e69-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8e69-176">The following is an example of the response.</span></span>

> <span data-ttu-id="b8e69-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8e69-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
