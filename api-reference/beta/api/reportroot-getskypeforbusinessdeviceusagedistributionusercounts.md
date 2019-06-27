---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7b151a72a015606f1fb2246e3561478daee30222
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265216"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="d42d9-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d42d9-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d42d9-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d42d9-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="d42d9-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="d42d9-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="d42d9-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="d42d9-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="d42d9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d42d9-108">Permissions</span></span>

<span data-ttu-id="d42d9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d42d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d42d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d42d9-111">Permission type</span></span>                        | <span data-ttu-id="d42d9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d42d9-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d42d9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d42d9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d42d9-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d42d9-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d42d9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d42d9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d42d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d42d9-116">Not supported.</span></span>                           |
| <span data-ttu-id="d42d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d42d9-117">Application</span></span>                            | <span data-ttu-id="d42d9-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d42d9-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d42d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d42d9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d42d9-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d42d9-120">Function parameters</span></span>

<span data-ttu-id="d42d9-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d42d9-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d42d9-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d42d9-122">Parameter</span></span> | <span data-ttu-id="d42d9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d42d9-123">Type</span></span>   | <span data-ttu-id="d42d9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d42d9-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d42d9-125">ponto</span><span class="sxs-lookup"><span data-stu-id="d42d9-125">period</span></span>    | <span data-ttu-id="d42d9-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d42d9-126">string</span></span> | <span data-ttu-id="d42d9-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d42d9-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d42d9-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d42d9-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d42d9-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d42d9-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d42d9-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d42d9-130">Required.</span></span> |

<span data-ttu-id="d42d9-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d42d9-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d42d9-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d42d9-132">The default output type is text/csv.</span></span> <span data-ttu-id="d42d9-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d42d9-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d42d9-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d42d9-134">Request headers</span></span>

| <span data-ttu-id="d42d9-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d42d9-135">Name</span></span>          | <span data-ttu-id="d42d9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d42d9-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d42d9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d42d9-137">Authorization</span></span> | <span data-ttu-id="d42d9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d42d9-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d42d9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d42d9-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d42d9-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d42d9-141">CSV</span></span>

<span data-ttu-id="d42d9-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d42d9-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d42d9-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d42d9-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d42d9-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d42d9-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d42d9-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d42d9-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d42d9-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d42d9-146">Report Refresh Date</span></span>
- <span data-ttu-id="d42d9-147">Windows</span><span class="sxs-lookup"><span data-stu-id="d42d9-147">Windows</span></span>
- <span data-ttu-id="d42d9-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d42d9-148">Windows Phone</span></span>
- <span data-ttu-id="d42d9-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d42d9-149">Android Phone</span></span>
- <span data-ttu-id="d42d9-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="d42d9-150">iPhone</span></span>
- <span data-ttu-id="d42d9-151">iPad</span><span class="sxs-lookup"><span data-stu-id="d42d9-151">iPad</span></span>
- <span data-ttu-id="d42d9-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d42d9-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d42d9-153">JSON</span><span class="sxs-lookup"><span data-stu-id="d42d9-153">JSON</span></span>

<span data-ttu-id="d42d9-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d42d9-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d42d9-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d42d9-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d42d9-156">CSV</span><span class="sxs-lookup"><span data-stu-id="d42d9-156">CSV</span></span>

<span data-ttu-id="d42d9-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d42d9-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d42d9-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d42d9-158">Request</span></span>

<span data-ttu-id="d42d9-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d42d9-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="d42d9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="d42d9-160">Response</span></span>

<span data-ttu-id="d42d9-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d42d9-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d42d9-162">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="d42d9-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d42d9-163">C#</span><span class="sxs-lookup"><span data-stu-id="d42d9-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d42d9-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="d42d9-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d42d9-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d42d9-165">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="d42d9-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d42d9-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="d42d9-167">JSON</span><span class="sxs-lookup"><span data-stu-id="d42d9-167">JSON</span></span>

<span data-ttu-id="d42d9-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d42d9-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d42d9-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d42d9-169">Request</span></span>

<span data-ttu-id="d42d9-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d42d9-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="d42d9-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d42d9-171">Response</span></span>

<span data-ttu-id="d42d9-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d42d9-172">The following is an example of the response.</span></span>

> <span data-ttu-id="d42d9-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d42d9-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d42d9-175">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d42d9-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d42d9-176">C#</span><span class="sxs-lookup"><span data-stu-id="d42d9-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d42d9-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="d42d9-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d42d9-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d42d9-178">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
