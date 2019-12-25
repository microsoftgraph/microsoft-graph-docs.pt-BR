---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e59c7c82192e287d00ccb1ae4582416955588c47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868944"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="2e4d3-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2e4d3-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e4d3-104">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e4d3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e4d3-105">Permissions</span></span>

<span data-ttu-id="2e4d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e4d3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e4d3-108">Permission type</span></span>                        | <span data-ttu-id="2e4d3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e4d3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2e4d3-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e4d3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e4d3-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e4d3-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2e4d3-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e4d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e4d3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-113">Not supported.</span></span>                           |
| <span data-ttu-id="2e4d3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e4d3-114">Application</span></span>                            | <span data-ttu-id="2e4d3-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e4d3-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="2e4d3-116">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2e4d3-117">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2e4d3-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2e4d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4d3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="2e4d3-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2e4d3-119">Function parameters</span></span>

<span data-ttu-id="2e4d3-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2e4d3-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2e4d3-121">Parameter</span></span> | <span data-ttu-id="2e4d3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e4d3-122">Type</span></span>   | <span data-ttu-id="2e4d3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e4d3-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2e4d3-124">ponto</span><span class="sxs-lookup"><span data-stu-id="2e4d3-124">period</span></span>    | <span data-ttu-id="2e4d3-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e4d3-125">string</span></span> | <span data-ttu-id="2e4d3-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2e4d3-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2e4d3-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2e4d3-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-129">Required.</span></span> |

<span data-ttu-id="2e4d3-130">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2e4d3-131">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-131">The default output type is text/csv.</span></span> <span data-ttu-id="2e4d3-132">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e4d3-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4d3-133">Request headers</span></span>

| <span data-ttu-id="2e4d3-134">Nome</span><span class="sxs-lookup"><span data-stu-id="2e4d3-134">Name</span></span>          | <span data-ttu-id="2e4d3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e4d3-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2e4d3-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e4d3-136">Authorization</span></span> | <span data-ttu-id="2e4d3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2e4d3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4d3-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2e4d3-140">CSV</span><span class="sxs-lookup"><span data-stu-id="2e4d3-140">CSV</span></span>

<span data-ttu-id="2e4d3-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2e4d3-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2e4d3-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2e4d3-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2e4d3-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2e4d3-145">Report Refresh Date</span></span>
- <span data-ttu-id="2e4d3-146">Web</span><span class="sxs-lookup"><span data-stu-id="2e4d3-146">Web</span></span>
- <span data-ttu-id="2e4d3-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="2e4d3-147">Windows Phone</span></span>
- <span data-ttu-id="2e4d3-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="2e4d3-148">Android Phone</span></span>
- <span data-ttu-id="2e4d3-149">iOS</span><span class="sxs-lookup"><span data-stu-id="2e4d3-149">iOS</span></span>
- <span data-ttu-id="2e4d3-150">Mac</span><span class="sxs-lookup"><span data-stu-id="2e4d3-150">Mac</span></span>
- <span data-ttu-id="2e4d3-151">Windows</span><span class="sxs-lookup"><span data-stu-id="2e4d3-151">Windows</span></span>
- <span data-ttu-id="2e4d3-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2e4d3-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2e4d3-153">JSON</span><span class="sxs-lookup"><span data-stu-id="2e4d3-153">JSON</span></span>

<span data-ttu-id="2e4d3-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4d3-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e4d3-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2e4d3-156">CSV</span><span class="sxs-lookup"><span data-stu-id="2e4d3-156">CSV</span></span>

<span data-ttu-id="2e4d3-157">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2e4d3-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4d3-158">Request</span></span>

<span data-ttu-id="2e4d3-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e4d3-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4d3-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e4d3-161">C#</span><span class="sxs-lookup"><span data-stu-id="2e4d3-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e4d3-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4d3-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e4d3-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4d3-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2e4d3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4d3-164">Response</span></span>

<span data-ttu-id="2e4d3-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2e4d3-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2e4d3-167">JSON</span><span class="sxs-lookup"><span data-stu-id="2e4d3-167">JSON</span></span>

<span data-ttu-id="2e4d3-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2e4d3-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4d3-169">Request</span></span>

<span data-ttu-id="2e4d3-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e4d3-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4d3-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e4d3-172">C#</span><span class="sxs-lookup"><span data-stu-id="2e4d3-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e4d3-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4d3-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e4d3-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4d3-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2e4d3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4d3-175">Response</span></span>

<span data-ttu-id="2e4d3-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-176">The following is an example of the response.</span></span>

> <span data-ttu-id="2e4d3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e4d3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
