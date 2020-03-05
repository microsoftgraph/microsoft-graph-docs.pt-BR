---
title: 'reportRoot: getSharePointSiteUsagePages'
description: Obtenha o número de páginas visualizadas em todos os sites.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d3bcbe52dae25add3884f59f01a301f906cbab81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454224"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="68bfd-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="68bfd-103">reportRoot: getSharePointSiteUsagePages</span></span>

<span data-ttu-id="68bfd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68bfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68bfd-105">Obtenha o número de páginas visualizadas em todos os sites.</span><span class="sxs-lookup"><span data-stu-id="68bfd-105">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="68bfd-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="68bfd-106">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="68bfd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="68bfd-107">Permissions</span></span>

<span data-ttu-id="68bfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68bfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68bfd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68bfd-110">Permission type</span></span>                        | <span data-ttu-id="68bfd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68bfd-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="68bfd-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68bfd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="68bfd-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="68bfd-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="68bfd-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68bfd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68bfd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68bfd-115">Not supported.</span></span>                           |
| <span data-ttu-id="68bfd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68bfd-116">Application</span></span>                            | <span data-ttu-id="68bfd-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="68bfd-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="68bfd-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="68bfd-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="68bfd-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="68bfd-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="68bfd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68bfd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="68bfd-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="68bfd-121">Function parameters</span></span>

<span data-ttu-id="68bfd-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="68bfd-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="68bfd-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="68bfd-123">Parameter</span></span> | <span data-ttu-id="68bfd-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="68bfd-124">Type</span></span>   | <span data-ttu-id="68bfd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="68bfd-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="68bfd-126">ponto</span><span class="sxs-lookup"><span data-stu-id="68bfd-126">period</span></span>    | <span data-ttu-id="68bfd-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68bfd-127">string</span></span> | <span data-ttu-id="68bfd-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="68bfd-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="68bfd-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="68bfd-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="68bfd-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="68bfd-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="68bfd-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68bfd-131">Required.</span></span> |

<span data-ttu-id="68bfd-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="68bfd-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="68bfd-133">The default output type is text/csv.</span></span> <span data-ttu-id="68bfd-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="68bfd-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68bfd-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-135">Request headers</span></span>

| <span data-ttu-id="68bfd-136">Nome</span><span class="sxs-lookup"><span data-stu-id="68bfd-136">Name</span></span>          | <span data-ttu-id="68bfd-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="68bfd-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="68bfd-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="68bfd-138">Authorization</span></span> | <span data-ttu-id="68bfd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68bfd-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="68bfd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="68bfd-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="68bfd-142">CSV</span><span class="sxs-lookup"><span data-stu-id="68bfd-142">CSV</span></span>

<span data-ttu-id="68bfd-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="68bfd-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="68bfd-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="68bfd-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="68bfd-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="68bfd-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="68bfd-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="68bfd-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="68bfd-147">Report Refresh Date</span></span>
- <span data-ttu-id="68bfd-148">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="68bfd-148">Site Type</span></span>
- <span data-ttu-id="68bfd-149">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="68bfd-149">Page View Count</span></span>
- <span data-ttu-id="68bfd-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="68bfd-150">Report Date</span></span>
- <span data-ttu-id="68bfd-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="68bfd-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="68bfd-152">JSON</span><span class="sxs-lookup"><span data-stu-id="68bfd-152">JSON</span></span>

<span data-ttu-id="68bfd-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68bfd-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68bfd-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="68bfd-155">CSV</span><span class="sxs-lookup"><span data-stu-id="68bfd-155">CSV</span></span>

<span data-ttu-id="68bfd-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="68bfd-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="68bfd-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-157">Request</span></span>

<span data-ttu-id="68bfd-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68bfd-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="68bfd-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="68bfd-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="68bfd-160">C#</span><span class="sxs-lookup"><span data-stu-id="68bfd-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagepages-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68bfd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68bfd-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagepages-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68bfd-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68bfd-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagepages-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="68bfd-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="68bfd-163">Response</span></span>

<span data-ttu-id="68bfd-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="68bfd-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="68bfd-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="68bfd-166">JSON</span><span class="sxs-lookup"><span data-stu-id="68bfd-166">JSON</span></span>

<span data-ttu-id="68bfd-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="68bfd-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="68bfd-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68bfd-168">Request</span></span>

<span data-ttu-id="68bfd-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68bfd-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="68bfd-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="68bfd-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="68bfd-171">C#</span><span class="sxs-lookup"><span data-stu-id="68bfd-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagepages-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68bfd-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68bfd-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagepages-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68bfd-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68bfd-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagepages-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="68bfd-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="68bfd-174">Response</span></span>

<span data-ttu-id="68bfd-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68bfd-175">The following is an example of the response.</span></span>

> <span data-ttu-id="68bfd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68bfd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsagePages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "pageViewCount": 183, 
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
