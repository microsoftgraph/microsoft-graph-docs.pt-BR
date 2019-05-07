---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Obtenha dados sobre o uso do dispositivo Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9c975ba4cc4a31135f71984faa269c3c15fb70d8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639219"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="cf8d7-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="cf8d7-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf8d7-104">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="cf8d7-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="cf8d7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf8d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf8d7-106">Permissions</span></span>

<span data-ttu-id="cf8d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf8d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf8d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf8d7-109">Permission type</span></span>                        | <span data-ttu-id="cf8d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf8d7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf8d7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf8d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf8d7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8d7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf8d7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf8d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf8d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-114">Not supported.</span></span>                           |
| <span data-ttu-id="cf8d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf8d7-115">Application</span></span>                            | <span data-ttu-id="cf8d7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf8d7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cf8d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf8d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="cf8d7-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cf8d7-118">Function parameters</span></span>

<span data-ttu-id="cf8d7-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="cf8d7-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cf8d7-120">Parameter</span></span> | <span data-ttu-id="cf8d7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf8d7-121">Type</span></span>   | <span data-ttu-id="cf8d7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf8d7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf8d7-123">ponto</span><span class="sxs-lookup"><span data-stu-id="cf8d7-123">period</span></span>    | <span data-ttu-id="cf8d7-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf8d7-124">string</span></span> | <span data-ttu-id="cf8d7-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf8d7-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf8d7-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="cf8d7-128">data</span><span class="sxs-lookup"><span data-stu-id="cf8d7-128">date</span></span>      | <span data-ttu-id="cf8d7-129">Data</span><span class="sxs-lookup"><span data-stu-id="cf8d7-129">Date</span></span>   | <span data-ttu-id="cf8d7-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="cf8d7-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="cf8d7-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="cf8d7-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="cf8d7-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cf8d7-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-135">The default output type is text/csv.</span></span> <span data-ttu-id="cf8d7-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf8d7-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8d7-137">Request headers</span></span>

| <span data-ttu-id="cf8d7-138">Nome</span><span class="sxs-lookup"><span data-stu-id="cf8d7-138">Name</span></span>          | <span data-ttu-id="cf8d7-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf8d7-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf8d7-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf8d7-140">Authorization</span></span> | <span data-ttu-id="cf8d7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf8d7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf8d7-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cf8d7-144">CSV</span><span class="sxs-lookup"><span data-stu-id="cf8d7-144">CSV</span></span>

<span data-ttu-id="cf8d7-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf8d7-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf8d7-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf8d7-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cf8d7-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cf8d7-149">Report Refresh Date</span></span>
- <span data-ttu-id="cf8d7-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="cf8d7-150">User Principal Name</span></span>
- <span data-ttu-id="cf8d7-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="cf8d7-151">Display Name</span></span>
- <span data-ttu-id="cf8d7-152">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="cf8d7-152">User State</span></span>
- <span data-ttu-id="cf8d7-153">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="cf8d7-153">State Change Date</span></span>
- <span data-ttu-id="cf8d7-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="cf8d7-154">Last Activity Date</span></span>
- <span data-ttu-id="cf8d7-155">Usou Web</span><span class="sxs-lookup"><span data-stu-id="cf8d7-155">Used Web</span></span>
- <span data-ttu-id="cf8d7-156">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="cf8d7-156">Used Windows Phone</span></span>
- <span data-ttu-id="cf8d7-157">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="cf8d7-157">Used Android Phone</span></span>
- <span data-ttu-id="cf8d7-158">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="cf8d7-158">Used iPhone</span></span>
- <span data-ttu-id="cf8d7-159">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="cf8d7-159">Used iPad</span></span>
- <span data-ttu-id="cf8d7-160">Usou outros</span><span class="sxs-lookup"><span data-stu-id="cf8d7-160">Used Others</span></span>
- <span data-ttu-id="cf8d7-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cf8d7-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cf8d7-162">JSON</span><span class="sxs-lookup"><span data-stu-id="cf8d7-162">JSON</span></span>

<span data-ttu-id="cf8d7-163">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="cf8d7-164">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="cf8d7-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf8d7-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cf8d7-166">CSV</span><span class="sxs-lookup"><span data-stu-id="cf8d7-166">CSV</span></span>

<span data-ttu-id="cf8d7-167">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cf8d7-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8d7-168">Request</span></span>

<span data-ttu-id="cf8d7-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cf8d7-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf8d7-170">Response</span></span>

<span data-ttu-id="cf8d7-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf8d7-172">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cf8d7-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf8d7-173">Basic</span><span class="sxs-lookup"><span data-stu-id="cf8d7-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf8d7-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf8d7-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="cf8d7-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="cf8d7-176">JSON</span><span class="sxs-lookup"><span data-stu-id="cf8d7-176">JSON</span></span>

<span data-ttu-id="cf8d7-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cf8d7-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf8d7-178">Request</span></span>

<span data-ttu-id="cf8d7-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cf8d7-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf8d7-180">Response</span></span>

<span data-ttu-id="cf8d7-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-181">The following is an example of the response.</span></span>

> <span data-ttu-id="cf8d7-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf8d7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cf8d7-184">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="cf8d7-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cf8d7-185">Basic</span><span class="sxs-lookup"><span data-stu-id="cf8d7-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf8d7-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf8d7-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
