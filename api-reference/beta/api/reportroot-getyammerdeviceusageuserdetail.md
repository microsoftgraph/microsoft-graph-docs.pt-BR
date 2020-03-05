---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Obtenha dados sobre o uso do dispositivo Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a33732ec7ba8ae08d8fd16d40d730483305576ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453972"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="03394-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="03394-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="03394-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03394-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03394-105">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="03394-105">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="03394-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="03394-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="03394-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="03394-107">Permissions</span></span>

<span data-ttu-id="03394-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03394-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03394-110">Permission type</span></span>                        | <span data-ttu-id="03394-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03394-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="03394-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03394-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="03394-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03394-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="03394-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03394-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03394-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03394-115">Not supported.</span></span>                           |
| <span data-ttu-id="03394-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03394-116">Application</span></span>                            | <span data-ttu-id="03394-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="03394-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="03394-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="03394-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="03394-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="03394-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="03394-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03394-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="03394-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="03394-121">Function parameters</span></span>

<span data-ttu-id="03394-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="03394-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="03394-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="03394-123">Parameter</span></span> | <span data-ttu-id="03394-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="03394-124">Type</span></span>   | <span data-ttu-id="03394-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="03394-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="03394-126">ponto</span><span class="sxs-lookup"><span data-stu-id="03394-126">period</span></span>    | <span data-ttu-id="03394-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03394-127">string</span></span> | <span data-ttu-id="03394-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="03394-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="03394-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="03394-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="03394-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="03394-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="03394-131">data</span><span class="sxs-lookup"><span data-stu-id="03394-131">date</span></span>      | <span data-ttu-id="03394-132">Data</span><span class="sxs-lookup"><span data-stu-id="03394-132">Date</span></span>   | <span data-ttu-id="03394-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="03394-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="03394-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="03394-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="03394-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="03394-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="03394-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="03394-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="03394-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="03394-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="03394-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="03394-138">The default output type is text/csv.</span></span> <span data-ttu-id="03394-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="03394-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03394-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03394-140">Request headers</span></span>

| <span data-ttu-id="03394-141">Nome</span><span class="sxs-lookup"><span data-stu-id="03394-141">Name</span></span>          | <span data-ttu-id="03394-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="03394-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="03394-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="03394-143">Authorization</span></span> | <span data-ttu-id="03394-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03394-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="03394-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="03394-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="03394-147">CSV</span><span class="sxs-lookup"><span data-stu-id="03394-147">CSV</span></span>

<span data-ttu-id="03394-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="03394-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="03394-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="03394-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="03394-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="03394-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="03394-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="03394-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="03394-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="03394-152">Report Refresh Date</span></span>
- <span data-ttu-id="03394-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="03394-153">User Principal Name</span></span>
- <span data-ttu-id="03394-154">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="03394-154">Display Name</span></span>
- <span data-ttu-id="03394-155">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="03394-155">User State</span></span>
- <span data-ttu-id="03394-156">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="03394-156">State Change Date</span></span>
- <span data-ttu-id="03394-157">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="03394-157">Last Activity Date</span></span>
- <span data-ttu-id="03394-158">Usou Web</span><span class="sxs-lookup"><span data-stu-id="03394-158">Used Web</span></span>
- <span data-ttu-id="03394-159">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="03394-159">Used Windows Phone</span></span>
- <span data-ttu-id="03394-160">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="03394-160">Used Android Phone</span></span>
- <span data-ttu-id="03394-161">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="03394-161">Used iPhone</span></span>
- <span data-ttu-id="03394-162">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="03394-162">Used iPad</span></span>
- <span data-ttu-id="03394-163">Usou outros</span><span class="sxs-lookup"><span data-stu-id="03394-163">Used Others</span></span>
- <span data-ttu-id="03394-164">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="03394-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="03394-165">JSON</span><span class="sxs-lookup"><span data-stu-id="03394-165">JSON</span></span>

<span data-ttu-id="03394-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03394-166">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="03394-167">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="03394-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="03394-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03394-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="03394-169">CSV</span><span class="sxs-lookup"><span data-stu-id="03394-169">CSV</span></span>

<span data-ttu-id="03394-170">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="03394-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="03394-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03394-171">Request</span></span>

<span data-ttu-id="03394-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03394-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03394-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="03394-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="03394-174">C#</span><span class="sxs-lookup"><span data-stu-id="03394-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03394-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03394-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03394-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03394-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03394-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="03394-177">Response</span></span>

<span data-ttu-id="03394-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03394-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="03394-179">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="03394-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="03394-180">JSON</span><span class="sxs-lookup"><span data-stu-id="03394-180">JSON</span></span>

<span data-ttu-id="03394-181">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="03394-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="03394-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03394-182">Request</span></span>

<span data-ttu-id="03394-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03394-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03394-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="03394-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="03394-185">C#</span><span class="sxs-lookup"><span data-stu-id="03394-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03394-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03394-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03394-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03394-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03394-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="03394-188">Response</span></span>

<span data-ttu-id="03394-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03394-189">The following is an example of the response.</span></span>

> <span data-ttu-id="03394-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03394-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
