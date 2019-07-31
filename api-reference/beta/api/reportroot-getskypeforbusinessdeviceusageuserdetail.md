---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cb9a2e6122ac4cb46d38d4ef1935140fc00fe34f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991881"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="45a30-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="45a30-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a30-104">Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="45a30-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="45a30-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="45a30-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="45a30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45a30-106">Permissions</span></span>

<span data-ttu-id="45a30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45a30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a30-109">Permission type</span></span>                        | <span data-ttu-id="45a30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45a30-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="45a30-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a30-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45a30-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45a30-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="45a30-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45a30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a30-114">Not supported.</span></span>                           |
| <span data-ttu-id="45a30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a30-115">Application</span></span>                            | <span data-ttu-id="45a30-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45a30-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="45a30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a30-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="45a30-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="45a30-118">Function parameters</span></span>

<span data-ttu-id="45a30-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="45a30-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="45a30-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="45a30-120">Parameter</span></span> | <span data-ttu-id="45a30-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a30-121">Type</span></span>   | <span data-ttu-id="45a30-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a30-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="45a30-123">ponto</span><span class="sxs-lookup"><span data-stu-id="45a30-123">period</span></span>    | <span data-ttu-id="45a30-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a30-124">string</span></span> | <span data-ttu-id="45a30-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="45a30-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="45a30-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="45a30-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="45a30-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="45a30-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="45a30-128">data</span><span class="sxs-lookup"><span data-stu-id="45a30-128">date</span></span>      | <span data-ttu-id="45a30-129">Data</span><span class="sxs-lookup"><span data-stu-id="45a30-129">Date</span></span>   | <span data-ttu-id="45a30-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="45a30-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="45a30-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="45a30-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="45a30-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="45a30-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="45a30-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="45a30-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="45a30-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="45a30-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="45a30-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="45a30-135">The default output type is text/csv.</span></span> <span data-ttu-id="45a30-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="45a30-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45a30-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a30-137">Request headers</span></span>

| <span data-ttu-id="45a30-138">Nome</span><span class="sxs-lookup"><span data-stu-id="45a30-138">Name</span></span>          | <span data-ttu-id="45a30-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a30-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="45a30-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a30-140">Authorization</span></span> | <span data-ttu-id="45a30-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a30-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="45a30-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a30-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="45a30-144">CSV</span><span class="sxs-lookup"><span data-stu-id="45a30-144">CSV</span></span>

<span data-ttu-id="45a30-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="45a30-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="45a30-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="45a30-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="45a30-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="45a30-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="45a30-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="45a30-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="45a30-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="45a30-149">Report Refresh Date</span></span>
- <span data-ttu-id="45a30-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="45a30-150">User Principal Name</span></span>
- <span data-ttu-id="45a30-151">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="45a30-151">Last Activity Date</span></span>
- <span data-ttu-id="45a30-152">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="45a30-152">Used Windows</span></span>
- <span data-ttu-id="45a30-153">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="45a30-153">Used Windows Phone</span></span>
- <span data-ttu-id="45a30-154">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="45a30-154">Used Android Phone</span></span>
- <span data-ttu-id="45a30-155">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="45a30-155">Used iPhone</span></span>
- <span data-ttu-id="45a30-156">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="45a30-156">Used iPad</span></span>
- <span data-ttu-id="45a30-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="45a30-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="45a30-158">JSON</span><span class="sxs-lookup"><span data-stu-id="45a30-158">JSON</span></span>

<span data-ttu-id="45a30-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a30-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="45a30-160">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="45a30-160">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="45a30-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45a30-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="45a30-162">CSV</span><span class="sxs-lookup"><span data-stu-id="45a30-162">CSV</span></span>

<span data-ttu-id="45a30-163">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="45a30-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="45a30-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a30-164">Request</span></span>

<span data-ttu-id="45a30-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a30-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45a30-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a30-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45a30-167">C#</span><span class="sxs-lookup"><span data-stu-id="45a30-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45a30-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="45a30-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45a30-169">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="45a30-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="45a30-170">Java</span><span class="sxs-lookup"><span data-stu-id="45a30-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45a30-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a30-171">Response</span></span>

<span data-ttu-id="45a30-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45a30-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="45a30-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="45a30-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="45a30-174">JSON</span><span class="sxs-lookup"><span data-stu-id="45a30-174">JSON</span></span>

<span data-ttu-id="45a30-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="45a30-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="45a30-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a30-176">Request</span></span>

<span data-ttu-id="45a30-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a30-177">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45a30-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a30-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45a30-179">C#</span><span class="sxs-lookup"><span data-stu-id="45a30-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45a30-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="45a30-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45a30-181">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="45a30-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="45a30-182">Java</span><span class="sxs-lookup"><span data-stu-id="45a30-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45a30-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a30-183">Response</span></span>

<span data-ttu-id="45a30-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45a30-184">The following is an example of the response.</span></span>

> <span data-ttu-id="45a30-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45a30-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
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
