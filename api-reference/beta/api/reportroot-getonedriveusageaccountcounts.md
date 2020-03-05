---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5522f4ca928b994d5db41adee692257826bb9b71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454287"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="62e03-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="62e03-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="62e03-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62e03-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62e03-106">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="62e03-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="62e03-107">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="62e03-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="62e03-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="62e03-108">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="62e03-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="62e03-109">Permissions</span></span>

<span data-ttu-id="62e03-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62e03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62e03-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62e03-112">Permission type</span></span>                        | <span data-ttu-id="62e03-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62e03-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62e03-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62e03-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="62e03-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e03-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62e03-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62e03-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62e03-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62e03-117">Not supported.</span></span>                           |
| <span data-ttu-id="62e03-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62e03-118">Application</span></span>                            | <span data-ttu-id="62e03-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e03-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="62e03-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="62e03-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="62e03-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="62e03-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="62e03-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62e03-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="62e03-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="62e03-123">Function parameters</span></span>

<span data-ttu-id="62e03-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="62e03-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="62e03-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="62e03-125">Parameter</span></span> | <span data-ttu-id="62e03-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="62e03-126">Type</span></span>   | <span data-ttu-id="62e03-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="62e03-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62e03-128">ponto</span><span class="sxs-lookup"><span data-stu-id="62e03-128">period</span></span>    | <span data-ttu-id="62e03-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62e03-129">string</span></span> | <span data-ttu-id="62e03-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="62e03-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62e03-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="62e03-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62e03-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="62e03-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="62e03-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62e03-133">Required.</span></span> |

<span data-ttu-id="62e03-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62e03-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="62e03-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="62e03-135">The default output type is text/csv.</span></span> <span data-ttu-id="62e03-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="62e03-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62e03-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62e03-137">Request headers</span></span>

| <span data-ttu-id="62e03-138">Nome</span><span class="sxs-lookup"><span data-stu-id="62e03-138">Name</span></span>          | <span data-ttu-id="62e03-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="62e03-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="62e03-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="62e03-140">Authorization</span></span> | <span data-ttu-id="62e03-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62e03-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62e03-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="62e03-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="62e03-144">CSV</span><span class="sxs-lookup"><span data-stu-id="62e03-144">CSV</span></span>

<span data-ttu-id="62e03-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="62e03-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62e03-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="62e03-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62e03-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="62e03-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62e03-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="62e03-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="62e03-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="62e03-149">Report Refresh Date</span></span>
- <span data-ttu-id="62e03-150">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="62e03-150">Site Type</span></span>
- <span data-ttu-id="62e03-151">Total</span><span class="sxs-lookup"><span data-stu-id="62e03-151">Total</span></span>
- <span data-ttu-id="62e03-152">Ativo</span><span class="sxs-lookup"><span data-stu-id="62e03-152">Active</span></span>
- <span data-ttu-id="62e03-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="62e03-153">Report Date</span></span>
- <span data-ttu-id="62e03-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="62e03-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="62e03-155">JSON</span><span class="sxs-lookup"><span data-stu-id="62e03-155">JSON</span></span>

<span data-ttu-id="62e03-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62e03-156">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62e03-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62e03-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="62e03-158">CSV</span><span class="sxs-lookup"><span data-stu-id="62e03-158">CSV</span></span>

<span data-ttu-id="62e03-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="62e03-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="62e03-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62e03-160">Request</span></span>

<span data-ttu-id="62e03-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62e03-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62e03-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="62e03-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="62e03-163">C#</span><span class="sxs-lookup"><span data-stu-id="62e03-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62e03-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62e03-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62e03-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62e03-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62e03-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="62e03-166">Response</span></span>

<span data-ttu-id="62e03-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62e03-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="62e03-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="62e03-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="62e03-169">JSON</span><span class="sxs-lookup"><span data-stu-id="62e03-169">JSON</span></span>

<span data-ttu-id="62e03-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="62e03-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="62e03-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62e03-171">Request</span></span>

<span data-ttu-id="62e03-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62e03-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62e03-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="62e03-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="62e03-174">C#</span><span class="sxs-lookup"><span data-stu-id="62e03-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62e03-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62e03-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62e03-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62e03-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="62e03-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="62e03-177">Response</span></span>

<span data-ttu-id="62e03-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62e03-178">The following is an example of the response.</span></span>

> <span data-ttu-id="62e03-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62e03-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
