---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Obtenha dados sobre o uso do dispositivo Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e80aa5253d5548b6181395664a150420811b196d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867040"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="96c1e-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="96c1e-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96c1e-104">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="96c1e-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="96c1e-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="96c1e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="96c1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96c1e-106">Permissions</span></span>

<span data-ttu-id="96c1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96c1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96c1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96c1e-109">Permission type</span></span>                        | <span data-ttu-id="96c1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96c1e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="96c1e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96c1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96c1e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="96c1e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="96c1e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96c1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c1e-114">Not supported.</span></span>                           |
| <span data-ttu-id="96c1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96c1e-115">Application</span></span>                            | <span data-ttu-id="96c1e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="96c1e-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="96c1e-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="96c1e-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="96c1e-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="96c1e-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="96c1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96c1e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="96c1e-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="96c1e-120">Function parameters</span></span>

<span data-ttu-id="96c1e-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="96c1e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="96c1e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="96c1e-122">Parameter</span></span> | <span data-ttu-id="96c1e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="96c1e-123">Type</span></span>   | <span data-ttu-id="96c1e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c1e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="96c1e-125">ponto</span><span class="sxs-lookup"><span data-stu-id="96c1e-125">period</span></span>    | <span data-ttu-id="96c1e-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96c1e-126">string</span></span> | <span data-ttu-id="96c1e-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="96c1e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="96c1e-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="96c1e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="96c1e-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="96c1e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="96c1e-130">data</span><span class="sxs-lookup"><span data-stu-id="96c1e-130">date</span></span>      | <span data-ttu-id="96c1e-131">Data</span><span class="sxs-lookup"><span data-stu-id="96c1e-131">Date</span></span>   | <span data-ttu-id="96c1e-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="96c1e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="96c1e-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="96c1e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="96c1e-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="96c1e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="96c1e-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="96c1e-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="96c1e-136">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="96c1e-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="96c1e-137">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="96c1e-137">The default output type is text/csv.</span></span> <span data-ttu-id="96c1e-138">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="96c1e-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96c1e-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96c1e-139">Request headers</span></span>

| <span data-ttu-id="96c1e-140">Nome</span><span class="sxs-lookup"><span data-stu-id="96c1e-140">Name</span></span>          | <span data-ttu-id="96c1e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c1e-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="96c1e-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="96c1e-142">Authorization</span></span> | <span data-ttu-id="96c1e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96c1e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="96c1e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c1e-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="96c1e-146">CSV</span><span class="sxs-lookup"><span data-stu-id="96c1e-146">CSV</span></span>

<span data-ttu-id="96c1e-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="96c1e-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="96c1e-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="96c1e-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="96c1e-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="96c1e-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="96c1e-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="96c1e-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="96c1e-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="96c1e-151">Report Refresh Date</span></span>
- <span data-ttu-id="96c1e-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="96c1e-152">User Principal Name</span></span>
- <span data-ttu-id="96c1e-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="96c1e-153">Display Name</span></span>
- <span data-ttu-id="96c1e-154">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="96c1e-154">User State</span></span>
- <span data-ttu-id="96c1e-155">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="96c1e-155">State Change Date</span></span>
- <span data-ttu-id="96c1e-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="96c1e-156">Last Activity Date</span></span>
- <span data-ttu-id="96c1e-157">Usou Web</span><span class="sxs-lookup"><span data-stu-id="96c1e-157">Used Web</span></span>
- <span data-ttu-id="96c1e-158">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="96c1e-158">Used Windows Phone</span></span>
- <span data-ttu-id="96c1e-159">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="96c1e-159">Used Android Phone</span></span>
- <span data-ttu-id="96c1e-160">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="96c1e-160">Used iPhone</span></span>
- <span data-ttu-id="96c1e-161">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="96c1e-161">Used iPad</span></span>
- <span data-ttu-id="96c1e-162">Usou outros</span><span class="sxs-lookup"><span data-stu-id="96c1e-162">Used Others</span></span>
- <span data-ttu-id="96c1e-163">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="96c1e-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="96c1e-164">JSON</span><span class="sxs-lookup"><span data-stu-id="96c1e-164">JSON</span></span>

<span data-ttu-id="96c1e-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96c1e-165">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="96c1e-166">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="96c1e-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="96c1e-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96c1e-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="96c1e-168">CSV</span><span class="sxs-lookup"><span data-stu-id="96c1e-168">CSV</span></span>

<span data-ttu-id="96c1e-169">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="96c1e-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="96c1e-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96c1e-170">Request</span></span>

<span data-ttu-id="96c1e-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c1e-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96c1e-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="96c1e-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96c1e-173">C#</span><span class="sxs-lookup"><span data-stu-id="96c1e-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96c1e-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96c1e-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96c1e-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96c1e-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96c1e-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c1e-176">Response</span></span>

<span data-ttu-id="96c1e-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96c1e-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="96c1e-178">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="96c1e-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="96c1e-179">JSON</span><span class="sxs-lookup"><span data-stu-id="96c1e-179">JSON</span></span>

<span data-ttu-id="96c1e-180">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="96c1e-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="96c1e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96c1e-181">Request</span></span>

<span data-ttu-id="96c1e-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c1e-182">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="96c1e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="96c1e-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96c1e-184">C#</span><span class="sxs-lookup"><span data-stu-id="96c1e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96c1e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96c1e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96c1e-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96c1e-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96c1e-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c1e-187">Response</span></span>

<span data-ttu-id="96c1e-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96c1e-188">The following is an example of the response.</span></span>

> <span data-ttu-id="96c1e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96c1e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
