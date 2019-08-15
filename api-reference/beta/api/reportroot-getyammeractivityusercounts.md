---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 088a3f3ef57a92af4d79888d3327a4c8c18b7861
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411057"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="121e7-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="121e7-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="121e7-104">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="121e7-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="121e7-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="121e7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="121e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="121e7-106">Permissions</span></span>

<span data-ttu-id="121e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="121e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="121e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="121e7-109">Permission type</span></span>                        | <span data-ttu-id="121e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="121e7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="121e7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="121e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="121e7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="121e7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="121e7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="121e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="121e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="121e7-114">Not supported.</span></span>                           |
| <span data-ttu-id="121e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="121e7-115">Application</span></span>                            | <span data-ttu-id="121e7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="121e7-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="121e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="121e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="121e7-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="121e7-118">Function parameters</span></span>

<span data-ttu-id="121e7-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="121e7-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="121e7-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="121e7-120">Parameter</span></span> | <span data-ttu-id="121e7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="121e7-121">Type</span></span>   | <span data-ttu-id="121e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="121e7-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="121e7-123">ponto</span><span class="sxs-lookup"><span data-stu-id="121e7-123">period</span></span>    | <span data-ttu-id="121e7-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121e7-124">string</span></span> | <span data-ttu-id="121e7-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="121e7-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="121e7-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="121e7-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="121e7-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="121e7-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="121e7-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="121e7-128">Required.</span></span> |

<span data-ttu-id="121e7-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="121e7-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="121e7-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="121e7-130">The default output type is text/csv.</span></span> <span data-ttu-id="121e7-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="121e7-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="121e7-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="121e7-132">Request headers</span></span>

| <span data-ttu-id="121e7-133">Nome</span><span class="sxs-lookup"><span data-stu-id="121e7-133">Name</span></span>          | <span data-ttu-id="121e7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="121e7-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="121e7-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="121e7-135">Authorization</span></span> | <span data-ttu-id="121e7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="121e7-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="121e7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="121e7-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="121e7-139">CSV</span><span class="sxs-lookup"><span data-stu-id="121e7-139">CSV</span></span>

<span data-ttu-id="121e7-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="121e7-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="121e7-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="121e7-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="121e7-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="121e7-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="121e7-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="121e7-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="121e7-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="121e7-144">Report Refresh Date</span></span>
- <span data-ttu-id="121e7-145">Curtidos</span><span class="sxs-lookup"><span data-stu-id="121e7-145">Liked</span></span>
- <span data-ttu-id="121e7-146">Postados</span><span class="sxs-lookup"><span data-stu-id="121e7-146">Posted</span></span>
- <span data-ttu-id="121e7-147">Ler</span><span class="sxs-lookup"><span data-stu-id="121e7-147">Read</span></span>
- <span data-ttu-id="121e7-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="121e7-148">Report Date</span></span>
- <span data-ttu-id="121e7-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="121e7-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="121e7-150">JSON</span><span class="sxs-lookup"><span data-stu-id="121e7-150">JSON</span></span>

<span data-ttu-id="121e7-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="121e7-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="121e7-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="121e7-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="121e7-153">CSV</span><span class="sxs-lookup"><span data-stu-id="121e7-153">CSV</span></span>

<span data-ttu-id="121e7-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="121e7-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="121e7-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="121e7-155">Request</span></span>

<span data-ttu-id="121e7-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="121e7-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="121e7-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="121e7-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="121e7-158">C#</span><span class="sxs-lookup"><span data-stu-id="121e7-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="121e7-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="121e7-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="121e7-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="121e7-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="121e7-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="121e7-161">Response</span></span>

<span data-ttu-id="121e7-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="121e7-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="121e7-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="121e7-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="121e7-164">JSON</span><span class="sxs-lookup"><span data-stu-id="121e7-164">JSON</span></span>

<span data-ttu-id="121e7-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="121e7-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="121e7-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="121e7-166">Request</span></span>

<span data-ttu-id="121e7-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="121e7-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="121e7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="121e7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="121e7-169">C#</span><span class="sxs-lookup"><span data-stu-id="121e7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="121e7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="121e7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="121e7-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="121e7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="121e7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="121e7-172">Response</span></span>

<span data-ttu-id="121e7-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="121e7-173">The following is an example of the response.</span></span>

> <span data-ttu-id="121e7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="121e7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
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
