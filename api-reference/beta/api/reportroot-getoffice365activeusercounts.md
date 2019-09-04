---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 502faabe5a2484e491b530e186a3a07d7ff6ab0a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725301"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="9fd97-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="9fd97-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fd97-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="9fd97-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="9fd97-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="9fd97-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fd97-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fd97-106">Permissions</span></span>

<span data-ttu-id="9fd97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fd97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fd97-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fd97-109">Permission type</span></span>                        | <span data-ttu-id="9fd97-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fd97-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9fd97-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fd97-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fd97-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd97-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9fd97-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fd97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fd97-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fd97-114">Not supported.</span></span>                           |
| <span data-ttu-id="9fd97-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fd97-115">Application</span></span>                            | <span data-ttu-id="9fd97-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fd97-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9fd97-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd97-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9fd97-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9fd97-118">Function parameters</span></span>

<span data-ttu-id="9fd97-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9fd97-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9fd97-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9fd97-120">Parameter</span></span> | <span data-ttu-id="9fd97-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd97-121">Type</span></span>   | <span data-ttu-id="9fd97-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd97-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9fd97-123">ponto</span><span class="sxs-lookup"><span data-stu-id="9fd97-123">period</span></span>    | <span data-ttu-id="9fd97-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd97-124">string</span></span> | <span data-ttu-id="9fd97-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9fd97-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9fd97-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9fd97-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9fd97-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9fd97-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9fd97-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd97-128">Required.</span></span> |

<span data-ttu-id="9fd97-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd97-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9fd97-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9fd97-130">The default output type is text/csv.</span></span> <span data-ttu-id="9fd97-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd97-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fd97-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd97-132">Request headers</span></span>

| <span data-ttu-id="9fd97-133">Nome</span><span class="sxs-lookup"><span data-stu-id="9fd97-133">Name</span></span>          | <span data-ttu-id="9fd97-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd97-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9fd97-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fd97-135">Authorization</span></span> | <span data-ttu-id="9fd97-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd97-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9fd97-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd97-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9fd97-139">CSV</span><span class="sxs-lookup"><span data-stu-id="9fd97-139">CSV</span></span>

<span data-ttu-id="9fd97-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9fd97-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9fd97-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd97-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9fd97-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9fd97-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9fd97-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="9fd97-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="9fd97-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9fd97-144">Report Refresh Date</span></span>
- <span data-ttu-id="9fd97-145">Office 365</span><span class="sxs-lookup"><span data-stu-id="9fd97-145">Office 365</span></span>
- <span data-ttu-id="9fd97-146">Exchange</span><span class="sxs-lookup"><span data-stu-id="9fd97-146">Exchange</span></span>
- <span data-ttu-id="9fd97-147">OneDrive</span><span class="sxs-lookup"><span data-stu-id="9fd97-147">OneDrive</span></span>
- <span data-ttu-id="9fd97-148">SharePoint</span><span class="sxs-lookup"><span data-stu-id="9fd97-148">SharePoint</span></span>
- <span data-ttu-id="9fd97-149">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="9fd97-149">Skype For Business</span></span> 
- <span data-ttu-id="9fd97-150">Yammer</span><span class="sxs-lookup"><span data-stu-id="9fd97-150">Yammer</span></span>
- <span data-ttu-id="9fd97-151">Teams</span><span class="sxs-lookup"><span data-stu-id="9fd97-151">Teams</span></span>
- <span data-ttu-id="9fd97-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9fd97-152">Report Date</span></span>
- <span data-ttu-id="9fd97-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9fd97-153">Report Period</span></span>

<span data-ttu-id="9fd97-154">Não há suporte para as seguintes colunas no Microsoft Graph da China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="9fd97-154">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9fd97-155">Yammer</span><span class="sxs-lookup"><span data-stu-id="9fd97-155">Yammer</span></span>
- <span data-ttu-id="9fd97-156">Teams</span><span class="sxs-lookup"><span data-stu-id="9fd97-156">Teams</span></span>

### <a name="json"></a><span data-ttu-id="9fd97-157">JSON</span><span class="sxs-lookup"><span data-stu-id="9fd97-157">JSON</span></span>

<span data-ttu-id="9fd97-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd97-158">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="9fd97-159">As propriedades a seguir no objeto **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** não têm suporte no Microsoft Graph China operado pela 21vianet:</span><span class="sxs-lookup"><span data-stu-id="9fd97-159">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="9fd97-160">Yammer</span><span class="sxs-lookup"><span data-stu-id="9fd97-160">yammer</span></span>
- <span data-ttu-id="9fd97-161">Teams</span><span class="sxs-lookup"><span data-stu-id="9fd97-161">teams</span></span>

## <a name="example"></a><span data-ttu-id="9fd97-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fd97-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9fd97-163">CSV</span><span class="sxs-lookup"><span data-stu-id="9fd97-163">CSV</span></span>

<span data-ttu-id="9fd97-164">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="9fd97-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9fd97-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd97-165">Request</span></span>

<span data-ttu-id="9fd97-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fd97-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9fd97-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd97-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fd97-168">C#</span><span class="sxs-lookup"><span data-stu-id="9fd97-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fd97-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fd97-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fd97-170">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9fd97-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fd97-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd97-171">Response</span></span>

<span data-ttu-id="9fd97-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd97-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9fd97-173">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9fd97-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="9fd97-174">JSON</span><span class="sxs-lookup"><span data-stu-id="9fd97-174">JSON</span></span>

<span data-ttu-id="9fd97-175">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd97-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9fd97-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fd97-176">Request</span></span>

<span data-ttu-id="9fd97-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fd97-177">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9fd97-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd97-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fd97-179">C#</span><span class="sxs-lookup"><span data-stu-id="9fd97-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fd97-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fd97-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fd97-181">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9fd97-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fd97-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fd97-182">Response</span></span>

<span data-ttu-id="9fd97-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fd97-183">The following is an example of the response.</span></span>

> <span data-ttu-id="9fd97-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fd97-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
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
