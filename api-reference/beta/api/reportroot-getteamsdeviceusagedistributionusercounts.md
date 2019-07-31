---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 42f8d4f0d129ddaabc62ee22a9a37650d18ba32c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991797"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="d75f9-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d75f9-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d75f9-104">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="d75f9-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="d75f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d75f9-105">Permissions</span></span>

<span data-ttu-id="d75f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d75f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d75f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d75f9-108">Permission type</span></span>                        | <span data-ttu-id="d75f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d75f9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d75f9-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d75f9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d75f9-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d75f9-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d75f9-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d75f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d75f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d75f9-113">Not supported.</span></span>                           |
| <span data-ttu-id="d75f9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d75f9-114">Application</span></span>                            | <span data-ttu-id="d75f9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d75f9-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d75f9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d75f9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="d75f9-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d75f9-117">Function parameters</span></span>

<span data-ttu-id="d75f9-118">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d75f9-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d75f9-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d75f9-119">Parameter</span></span> | <span data-ttu-id="d75f9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d75f9-120">Type</span></span>   | <span data-ttu-id="d75f9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d75f9-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d75f9-122">ponto</span><span class="sxs-lookup"><span data-stu-id="d75f9-122">period</span></span>    | <span data-ttu-id="d75f9-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d75f9-123">string</span></span> | <span data-ttu-id="d75f9-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d75f9-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d75f9-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d75f9-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d75f9-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d75f9-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d75f9-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d75f9-127">Required.</span></span> |

<span data-ttu-id="d75f9-128">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d75f9-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d75f9-129">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d75f9-129">The default output type is text/csv.</span></span> <span data-ttu-id="d75f9-130">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d75f9-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d75f9-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d75f9-131">Request headers</span></span>

| <span data-ttu-id="d75f9-132">Nome</span><span class="sxs-lookup"><span data-stu-id="d75f9-132">Name</span></span>          | <span data-ttu-id="d75f9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d75f9-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d75f9-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="d75f9-134">Authorization</span></span> | <span data-ttu-id="d75f9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d75f9-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d75f9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d75f9-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d75f9-138">CSV</span><span class="sxs-lookup"><span data-stu-id="d75f9-138">CSV</span></span>

<span data-ttu-id="d75f9-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d75f9-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d75f9-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d75f9-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d75f9-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d75f9-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d75f9-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d75f9-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d75f9-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d75f9-143">Report Refresh Date</span></span>
- <span data-ttu-id="d75f9-144">Web</span><span class="sxs-lookup"><span data-stu-id="d75f9-144">Web</span></span>
- <span data-ttu-id="d75f9-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d75f9-145">Windows Phone</span></span>
- <span data-ttu-id="d75f9-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="d75f9-146">Android Phone</span></span>
- <span data-ttu-id="d75f9-147">iOS</span><span class="sxs-lookup"><span data-stu-id="d75f9-147">iOS</span></span>
- <span data-ttu-id="d75f9-148">Mac</span><span class="sxs-lookup"><span data-stu-id="d75f9-148">Mac</span></span>
- <span data-ttu-id="d75f9-149">Windows</span><span class="sxs-lookup"><span data-stu-id="d75f9-149">Windows</span></span>
- <span data-ttu-id="d75f9-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d75f9-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d75f9-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d75f9-151">JSON</span></span>

<span data-ttu-id="d75f9-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d75f9-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d75f9-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d75f9-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d75f9-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d75f9-154">CSV</span></span>

<span data-ttu-id="d75f9-155">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d75f9-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d75f9-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d75f9-156">Request</span></span>

<span data-ttu-id="d75f9-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d75f9-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d75f9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d75f9-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d75f9-159">C#</span><span class="sxs-lookup"><span data-stu-id="d75f9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d75f9-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="d75f9-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d75f9-161">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d75f9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d75f9-162">Java</span><span class="sxs-lookup"><span data-stu-id="d75f9-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d75f9-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d75f9-163">Response</span></span>

<span data-ttu-id="d75f9-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d75f9-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d75f9-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d75f9-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="d75f9-166">JSON</span><span class="sxs-lookup"><span data-stu-id="d75f9-166">JSON</span></span>

<span data-ttu-id="d75f9-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d75f9-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d75f9-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d75f9-168">Request</span></span>

<span data-ttu-id="d75f9-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d75f9-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d75f9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="d75f9-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d75f9-171">C#</span><span class="sxs-lookup"><span data-stu-id="d75f9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d75f9-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="d75f9-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d75f9-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d75f9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d75f9-174">Java</span><span class="sxs-lookup"><span data-stu-id="d75f9-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d75f9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d75f9-175">Response</span></span>

<span data-ttu-id="d75f9-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d75f9-176">The following is an example of the response.</span></span>

> <span data-ttu-id="d75f9-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d75f9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
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
