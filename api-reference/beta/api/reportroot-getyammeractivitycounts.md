---
title: 'reportRoot: getYammerActivityCounts'
description: Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f56273bf9c563e32d5e292ce31cb7c78a24590ef
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639107"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="137bb-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="137bb-103">reportRoot: getYammerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="137bb-104">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="137bb-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="137bb-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="137bb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="137bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="137bb-106">Permissions</span></span>

<span data-ttu-id="137bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="137bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="137bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="137bb-109">Permission type</span></span>                        | <span data-ttu-id="137bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="137bb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="137bb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="137bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="137bb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="137bb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="137bb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="137bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="137bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="137bb-114">Not supported.</span></span>                           |
| <span data-ttu-id="137bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="137bb-115">Application</span></span>                            | <span data-ttu-id="137bb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="137bb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="137bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="137bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="137bb-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="137bb-118">Function parameters</span></span>

<span data-ttu-id="137bb-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="137bb-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="137bb-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="137bb-120">Parameter</span></span> | <span data-ttu-id="137bb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="137bb-121">Type</span></span>   | <span data-ttu-id="137bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="137bb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="137bb-123">ponto</span><span class="sxs-lookup"><span data-stu-id="137bb-123">period</span></span>    | <span data-ttu-id="137bb-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="137bb-124">string</span></span> | <span data-ttu-id="137bb-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="137bb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="137bb-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="137bb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="137bb-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="137bb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="137bb-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="137bb-128">Required.</span></span> |

<span data-ttu-id="137bb-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="137bb-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="137bb-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="137bb-130">The default output type is text/csv.</span></span> <span data-ttu-id="137bb-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="137bb-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="137bb-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="137bb-132">Request headers</span></span>

| <span data-ttu-id="137bb-133">Nome</span><span class="sxs-lookup"><span data-stu-id="137bb-133">Name</span></span>          | <span data-ttu-id="137bb-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="137bb-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="137bb-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="137bb-135">Authorization</span></span> | <span data-ttu-id="137bb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="137bb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="137bb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="137bb-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="137bb-139">CSV</span><span class="sxs-lookup"><span data-stu-id="137bb-139">CSV</span></span>

<span data-ttu-id="137bb-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="137bb-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="137bb-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="137bb-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="137bb-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="137bb-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="137bb-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="137bb-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="137bb-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="137bb-144">Report Refresh Date</span></span>
- <span data-ttu-id="137bb-145">Curtidos</span><span class="sxs-lookup"><span data-stu-id="137bb-145">Liked</span></span>
- <span data-ttu-id="137bb-146">Postados</span><span class="sxs-lookup"><span data-stu-id="137bb-146">Posted</span></span>
- <span data-ttu-id="137bb-147">Ler</span><span class="sxs-lookup"><span data-stu-id="137bb-147">Read</span></span>
- <span data-ttu-id="137bb-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="137bb-148">Report Date</span></span>
- <span data-ttu-id="137bb-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="137bb-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="137bb-150">JSON</span><span class="sxs-lookup"><span data-stu-id="137bb-150">JSON</span></span>

<span data-ttu-id="137bb-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="137bb-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="137bb-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="137bb-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="137bb-153">CSV</span><span class="sxs-lookup"><span data-stu-id="137bb-153">CSV</span></span>

<span data-ttu-id="137bb-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="137bb-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="137bb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="137bb-155">Request</span></span>

<span data-ttu-id="137bb-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="137bb-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="137bb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="137bb-157">Response</span></span>

<span data-ttu-id="137bb-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="137bb-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="137bb-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="137bb-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="137bb-160">Basic</span><span class="sxs-lookup"><span data-stu-id="137bb-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="137bb-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="137bb-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="137bb-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="137bb-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="137bb-163">JSON</span><span class="sxs-lookup"><span data-stu-id="137bb-163">JSON</span></span>

<span data-ttu-id="137bb-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="137bb-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="137bb-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="137bb-165">Request</span></span>

<span data-ttu-id="137bb-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="137bb-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="137bb-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="137bb-167">Response</span></span>

<span data-ttu-id="137bb-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="137bb-168">The following is an example of the response.</span></span>

> <span data-ttu-id="137bb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="137bb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="137bb-171">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="137bb-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="137bb-172">Basic</span><span class="sxs-lookup"><span data-stu-id="137bb-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="137bb-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="137bb-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivitycounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
