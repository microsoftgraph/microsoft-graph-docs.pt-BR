---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a26d91c5fd1822e80c9e3a1e0ed476e13c900670
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454161"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="7aca4-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7aca4-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="7aca4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7aca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aca4-105">Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="7aca4-105">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="7aca4-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="7aca4-106">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="7aca4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aca4-107">Permissions</span></span>

<span data-ttu-id="7aca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7aca4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aca4-110">Permission type</span></span>                        | <span data-ttu-id="7aca4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aca4-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7aca4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aca4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aca4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aca4-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7aca4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aca4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aca4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aca4-115">Not supported.</span></span>                           |
| <span data-ttu-id="7aca4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aca4-116">Application</span></span>                            | <span data-ttu-id="7aca4-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aca4-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="7aca4-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7aca4-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7aca4-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7aca4-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7aca4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aca4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7aca4-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7aca4-121">Function parameters</span></span>

<span data-ttu-id="7aca4-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7aca4-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7aca4-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7aca4-123">Parameter</span></span> | <span data-ttu-id="7aca4-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aca4-124">Type</span></span>   | <span data-ttu-id="7aca4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aca4-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7aca4-126">ponto</span><span class="sxs-lookup"><span data-stu-id="7aca4-126">period</span></span>    | <span data-ttu-id="7aca4-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aca4-127">string</span></span> | <span data-ttu-id="7aca4-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7aca4-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7aca4-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7aca4-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7aca4-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7aca4-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7aca4-131">data</span><span class="sxs-lookup"><span data-stu-id="7aca4-131">date</span></span>      | <span data-ttu-id="7aca4-132">Data</span><span class="sxs-lookup"><span data-stu-id="7aca4-132">Date</span></span>   | <span data-ttu-id="7aca4-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="7aca4-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7aca4-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7aca4-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7aca4-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7aca4-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7aca4-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="7aca4-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="7aca4-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="7aca4-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7aca4-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="7aca4-138">The default output type is text/csv.</span></span> <span data-ttu-id="7aca4-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7aca4-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7aca4-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aca4-140">Request headers</span></span>

| <span data-ttu-id="7aca4-141">Nome</span><span class="sxs-lookup"><span data-stu-id="7aca4-141">Name</span></span>          | <span data-ttu-id="7aca4-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aca4-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7aca4-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aca4-143">Authorization</span></span> | <span data-ttu-id="7aca4-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aca4-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7aca4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aca4-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7aca4-147">CSV</span><span class="sxs-lookup"><span data-stu-id="7aca4-147">CSV</span></span>

<span data-ttu-id="7aca4-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7aca4-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7aca4-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7aca4-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7aca4-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7aca4-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7aca4-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7aca4-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7aca4-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7aca4-152">Report Refresh Date</span></span>
- <span data-ttu-id="7aca4-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="7aca4-153">User Principal Name</span></span>
- <span data-ttu-id="7aca4-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="7aca4-154">Last Activity Date</span></span>
- <span data-ttu-id="7aca4-155">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="7aca4-155">Used Windows</span></span>
- <span data-ttu-id="7aca4-156">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7aca4-156">Used Windows Phone</span></span>
- <span data-ttu-id="7aca4-157">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="7aca4-157">Used Android Phone</span></span>
- <span data-ttu-id="7aca4-158">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="7aca4-158">Used iPhone</span></span>
- <span data-ttu-id="7aca4-159">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="7aca4-159">Used iPad</span></span>
- <span data-ttu-id="7aca4-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7aca4-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7aca4-161">JSON</span><span class="sxs-lookup"><span data-stu-id="7aca4-161">JSON</span></span>

<span data-ttu-id="7aca4-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aca4-162">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="7aca4-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="7aca4-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="7aca4-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aca4-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7aca4-165">CSV</span><span class="sxs-lookup"><span data-stu-id="7aca4-165">CSV</span></span>

<span data-ttu-id="7aca4-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="7aca4-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7aca4-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aca4-167">Request</span></span>

<span data-ttu-id="7aca4-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aca4-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7aca4-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aca4-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="7aca4-170">C#</span><span class="sxs-lookup"><span data-stu-id="7aca4-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aca4-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aca4-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aca4-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aca4-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7aca4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aca4-173">Response</span></span>

<span data-ttu-id="7aca4-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aca4-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7aca4-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7aca4-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7aca4-176">JSON</span><span class="sxs-lookup"><span data-stu-id="7aca4-176">JSON</span></span>

<span data-ttu-id="7aca4-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="7aca4-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7aca4-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aca4-178">Request</span></span>

<span data-ttu-id="7aca4-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aca4-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7aca4-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="7aca4-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="7aca4-181">C#</span><span class="sxs-lookup"><span data-stu-id="7aca4-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7aca4-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7aca4-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7aca4-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7aca4-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7aca4-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aca4-184">Response</span></span>

<span data-ttu-id="7aca4-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aca4-185">The following is an example of the response.</span></span>

> <span data-ttu-id="7aca4-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aca4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
