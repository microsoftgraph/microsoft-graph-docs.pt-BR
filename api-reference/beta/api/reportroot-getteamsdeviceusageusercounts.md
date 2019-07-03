---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b13eca63f6b646270e37229920a03131447affd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446371"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="e4f65-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="e4f65-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f65-104">Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4f65-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f65-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4f65-105">Permissions</span></span>

<span data-ttu-id="e4f65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4f65-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4f65-108">Permission type</span></span>                        | <span data-ttu-id="e4f65-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4f65-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e4f65-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4f65-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4f65-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f65-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e4f65-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4f65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f65-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4f65-113">Not supported.</span></span>                           |
| <span data-ttu-id="e4f65-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4f65-114">Application</span></span>                            | <span data-ttu-id="e4f65-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4f65-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e4f65-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f65-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="e4f65-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e4f65-117">Function parameters</span></span>

<span data-ttu-id="e4f65-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e4f65-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e4f65-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e4f65-119">Parameter</span></span> | <span data-ttu-id="e4f65-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4f65-120">Type</span></span>   | <span data-ttu-id="e4f65-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f65-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e4f65-122">ponto</span><span class="sxs-lookup"><span data-stu-id="e4f65-122">period</span></span>    | <span data-ttu-id="e4f65-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4f65-123">string</span></span> | <span data-ttu-id="e4f65-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4f65-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e4f65-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e4f65-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e4f65-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e4f65-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e4f65-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4f65-127">Required.</span></span> |

<span data-ttu-id="e4f65-128">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f65-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e4f65-129">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e4f65-129">The default output type is text/csv.</span></span> <span data-ttu-id="e4f65-130">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f65-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4f65-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f65-131">Request headers</span></span>

| <span data-ttu-id="e4f65-132">Nome</span><span class="sxs-lookup"><span data-stu-id="e4f65-132">Name</span></span>          | <span data-ttu-id="e4f65-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4f65-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e4f65-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4f65-134">Authorization</span></span> | <span data-ttu-id="e4f65-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4f65-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e4f65-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f65-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e4f65-138">CSV</span><span class="sxs-lookup"><span data-stu-id="e4f65-138">CSV</span></span>

<span data-ttu-id="e4f65-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e4f65-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e4f65-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f65-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e4f65-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e4f65-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e4f65-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e4f65-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e4f65-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e4f65-143">Report Refresh Date</span></span>
- <span data-ttu-id="e4f65-144">Web</span><span class="sxs-lookup"><span data-stu-id="e4f65-144">Web</span></span>
- <span data-ttu-id="e4f65-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e4f65-145">Windows Phone</span></span>
- <span data-ttu-id="e4f65-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="e4f65-146">Android Phone</span></span>
- <span data-ttu-id="e4f65-147">iOS</span><span class="sxs-lookup"><span data-stu-id="e4f65-147">iOS</span></span>
- <span data-ttu-id="e4f65-148">Mac</span><span class="sxs-lookup"><span data-stu-id="e4f65-148">Mac</span></span>
- <span data-ttu-id="e4f65-149">Windows</span><span class="sxs-lookup"><span data-stu-id="e4f65-149">Windows</span></span>
- <span data-ttu-id="e4f65-150">Data do Relatório</span><span class="sxs-lookup"><span data-stu-id="e4f65-150">Report Date</span></span>
- <span data-ttu-id="e4f65-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e4f65-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e4f65-152">JSON</span><span class="sxs-lookup"><span data-stu-id="e4f65-152">JSON</span></span>

<span data-ttu-id="e4f65-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f65-153">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4f65-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4f65-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e4f65-155">CSV</span><span class="sxs-lookup"><span data-stu-id="e4f65-155">CSV</span></span>

<span data-ttu-id="e4f65-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e4f65-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e4f65-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f65-157">Request</span></span>

<span data-ttu-id="e4f65-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4f65-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e4f65-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f65-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4f65-160">C#</span><span class="sxs-lookup"><span data-stu-id="e4f65-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4f65-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4f65-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4f65-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e4f65-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4f65-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f65-163">Response</span></span>

<span data-ttu-id="e4f65-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f65-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e4f65-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e4f65-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e4f65-166">JSON</span><span class="sxs-lookup"><span data-stu-id="e4f65-166">JSON</span></span>

<span data-ttu-id="e4f65-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e4f65-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e4f65-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f65-168">Request</span></span>

<span data-ttu-id="e4f65-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4f65-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e4f65-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f65-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4f65-171">C#</span><span class="sxs-lookup"><span data-stu-id="e4f65-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4f65-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4f65-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4f65-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e4f65-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4f65-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f65-174">Response</span></span>

<span data-ttu-id="e4f65-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4f65-175">The following is an example of the response.</span></span>

> <span data-ttu-id="e4f65-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4f65-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
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
