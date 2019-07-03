---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0bf4fdadd5275a607b63392a4b2d28cfbf9d9f60
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446518"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="091dd-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="091dd-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="091dd-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="091dd-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="091dd-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="091dd-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="091dd-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="091dd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="091dd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="091dd-108">Permissions</span></span>

<span data-ttu-id="091dd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="091dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="091dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="091dd-111">Permission type</span></span>                        | <span data-ttu-id="091dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="091dd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="091dd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="091dd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="091dd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="091dd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="091dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="091dd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="091dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="091dd-116">Not supported.</span></span>                           |
| <span data-ttu-id="091dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="091dd-117">Application</span></span>                            | <span data-ttu-id="091dd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="091dd-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="091dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="091dd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="091dd-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="091dd-120">Function parameters</span></span>

<span data-ttu-id="091dd-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="091dd-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="091dd-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="091dd-122">Parameter</span></span> | <span data-ttu-id="091dd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="091dd-123">Type</span></span>   | <span data-ttu-id="091dd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="091dd-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="091dd-125">ponto</span><span class="sxs-lookup"><span data-stu-id="091dd-125">period</span></span>    | <span data-ttu-id="091dd-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="091dd-126">string</span></span> | <span data-ttu-id="091dd-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="091dd-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="091dd-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="091dd-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="091dd-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="091dd-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="091dd-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="091dd-130">Required.</span></span> |

<span data-ttu-id="091dd-131">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="091dd-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="091dd-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="091dd-132">The default output type is text/csv.</span></span> <span data-ttu-id="091dd-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="091dd-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="091dd-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="091dd-134">Request headers</span></span>

| <span data-ttu-id="091dd-135">Nome</span><span class="sxs-lookup"><span data-stu-id="091dd-135">Name</span></span>          | <span data-ttu-id="091dd-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="091dd-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="091dd-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="091dd-137">Authorization</span></span> | <span data-ttu-id="091dd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="091dd-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="091dd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="091dd-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="091dd-141">CSV</span><span class="sxs-lookup"><span data-stu-id="091dd-141">CSV</span></span>

<span data-ttu-id="091dd-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="091dd-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="091dd-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="091dd-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="091dd-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="091dd-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="091dd-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="091dd-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="091dd-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="091dd-146">Report Refresh Date</span></span>
- <span data-ttu-id="091dd-147">Windows</span><span class="sxs-lookup"><span data-stu-id="091dd-147">Windows</span></span>
- <span data-ttu-id="091dd-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="091dd-148">Windows Phone</span></span>
- <span data-ttu-id="091dd-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="091dd-149">Android Phone</span></span>
- <span data-ttu-id="091dd-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="091dd-150">iPhone</span></span>
- <span data-ttu-id="091dd-151">iPad</span><span class="sxs-lookup"><span data-stu-id="091dd-151">iPad</span></span>
- <span data-ttu-id="091dd-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="091dd-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="091dd-153">JSON</span><span class="sxs-lookup"><span data-stu-id="091dd-153">JSON</span></span>

<span data-ttu-id="091dd-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="091dd-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="091dd-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="091dd-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="091dd-156">CSV</span><span class="sxs-lookup"><span data-stu-id="091dd-156">CSV</span></span>

<span data-ttu-id="091dd-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="091dd-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="091dd-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="091dd-158">Request</span></span>

<span data-ttu-id="091dd-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="091dd-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="091dd-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="091dd-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="091dd-161">C#</span><span class="sxs-lookup"><span data-stu-id="091dd-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="091dd-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="091dd-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="091dd-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="091dd-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="091dd-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="091dd-164">Response</span></span>

<span data-ttu-id="091dd-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="091dd-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="091dd-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="091dd-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="091dd-167">JSON</span><span class="sxs-lookup"><span data-stu-id="091dd-167">JSON</span></span>

<span data-ttu-id="091dd-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="091dd-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="091dd-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="091dd-169">Request</span></span>

<span data-ttu-id="091dd-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="091dd-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="091dd-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="091dd-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="091dd-172">C#</span><span class="sxs-lookup"><span data-stu-id="091dd-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="091dd-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="091dd-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="091dd-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="091dd-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="091dd-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="091dd-175">Response</span></span>

<span data-ttu-id="091dd-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="091dd-176">The following is an example of the response.</span></span>

> <span data-ttu-id="091dd-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="091dd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
