---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e816f37e0bedbbbfa176fc2a8d6fac1c879bdec5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724983"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="3b1fd-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3b1fd-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1fd-105">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="3b1fd-106">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="3b1fd-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="3b1fd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1fd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b1fd-108">Permissions</span></span>

<span data-ttu-id="3b1fd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b1fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b1fd-111">Permission type</span></span>                        | <span data-ttu-id="3b1fd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b1fd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3b1fd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b1fd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b1fd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b1fd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3b1fd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b1fd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b1fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-116">Not supported.</span></span>                           |
| <span data-ttu-id="3b1fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b1fd-117">Application</span></span>                            | <span data-ttu-id="3b1fd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b1fd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3b1fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1fd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3b1fd-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3b1fd-120">Function parameters</span></span>

<span data-ttu-id="3b1fd-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3b1fd-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3b1fd-122">Parameter</span></span> | <span data-ttu-id="3b1fd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b1fd-123">Type</span></span>   | <span data-ttu-id="3b1fd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b1fd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3b1fd-125">ponto</span><span class="sxs-lookup"><span data-stu-id="3b1fd-125">period</span></span>    | <span data-ttu-id="3b1fd-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b1fd-126">string</span></span> | <span data-ttu-id="3b1fd-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3b1fd-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3b1fd-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3b1fd-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-130">Required.</span></span> |

<span data-ttu-id="3b1fd-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3b1fd-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-132">The default output type is text/csv.</span></span> <span data-ttu-id="3b1fd-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b1fd-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1fd-134">Request headers</span></span>

| <span data-ttu-id="3b1fd-135">Nome</span><span class="sxs-lookup"><span data-stu-id="3b1fd-135">Name</span></span>          | <span data-ttu-id="3b1fd-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b1fd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3b1fd-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b1fd-137">Authorization</span></span> | <span data-ttu-id="3b1fd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3b1fd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1fd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3b1fd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="3b1fd-141">CSV</span></span>

<span data-ttu-id="3b1fd-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3b1fd-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3b1fd-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3b1fd-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3b1fd-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3b1fd-146">Report Refresh Date</span></span>
- <span data-ttu-id="3b1fd-147">Windows</span><span class="sxs-lookup"><span data-stu-id="3b1fd-147">Windows</span></span>
- <span data-ttu-id="3b1fd-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3b1fd-148">Windows Phone</span></span>
- <span data-ttu-id="3b1fd-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="3b1fd-149">Android Phone</span></span>
- <span data-ttu-id="3b1fd-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="3b1fd-150">iPhone</span></span>
- <span data-ttu-id="3b1fd-151">iPad</span><span class="sxs-lookup"><span data-stu-id="3b1fd-151">iPad</span></span>
- <span data-ttu-id="3b1fd-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3b1fd-152">Report Date</span></span>
- <span data-ttu-id="3b1fd-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3b1fd-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3b1fd-154">JSON</span><span class="sxs-lookup"><span data-stu-id="3b1fd-154">JSON</span></span>

<span data-ttu-id="3b1fd-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b1fd-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b1fd-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3b1fd-157">CSV</span><span class="sxs-lookup"><span data-stu-id="3b1fd-157">CSV</span></span>

<span data-ttu-id="3b1fd-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3b1fd-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1fd-159">Request</span></span>

<span data-ttu-id="3b1fd-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3b1fd-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1fd-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b1fd-162">C#</span><span class="sxs-lookup"><span data-stu-id="3b1fd-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b1fd-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1fd-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b1fd-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3b1fd-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1fd-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1fd-165">Response</span></span>

<span data-ttu-id="3b1fd-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3b1fd-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="3b1fd-168">JSON</span><span class="sxs-lookup"><span data-stu-id="3b1fd-168">JSON</span></span>

<span data-ttu-id="3b1fd-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3b1fd-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b1fd-170">Request</span></span>

<span data-ttu-id="3b1fd-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3b1fd-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b1fd-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b1fd-173">C#</span><span class="sxs-lookup"><span data-stu-id="3b1fd-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b1fd-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b1fd-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b1fd-175">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3b1fd-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b1fd-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b1fd-176">Response</span></span>

<span data-ttu-id="3b1fd-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-177">The following is an example of the response.</span></span>

> <span data-ttu-id="3b1fd-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b1fd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
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
