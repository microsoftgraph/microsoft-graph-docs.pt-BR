---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 45d308c037d69fc845a0ede7289bfdfa0f322328
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639079"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="e6cdd-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e6cdd-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6cdd-104">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="e6cdd-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="e6cdd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6cdd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6cdd-106">Permissions</span></span>

<span data-ttu-id="e6cdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6cdd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6cdd-109">Permission type</span></span>                        | <span data-ttu-id="e6cdd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6cdd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6cdd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6cdd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6cdd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6cdd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6cdd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6cdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6cdd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-114">Not supported.</span></span>                           |
| <span data-ttu-id="e6cdd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6cdd-115">Application</span></span>                            | <span data-ttu-id="e6cdd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6cdd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e6cdd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6cdd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e6cdd-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e6cdd-118">Function parameters</span></span>

<span data-ttu-id="e6cdd-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e6cdd-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6cdd-120">Parameter</span></span> | <span data-ttu-id="e6cdd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6cdd-121">Type</span></span>   | <span data-ttu-id="e6cdd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cdd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6cdd-123">ponto</span><span class="sxs-lookup"><span data-stu-id="e6cdd-123">period</span></span>    | <span data-ttu-id="e6cdd-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6cdd-124">string</span></span> | <span data-ttu-id="e6cdd-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6cdd-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6cdd-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e6cdd-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-128">Required.</span></span> |

<span data-ttu-id="e6cdd-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e6cdd-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-130">The default output type is text/csv.</span></span> <span data-ttu-id="e6cdd-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6cdd-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cdd-132">Request headers</span></span>

| <span data-ttu-id="e6cdd-133">Nome</span><span class="sxs-lookup"><span data-stu-id="e6cdd-133">Name</span></span>          | <span data-ttu-id="e6cdd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6cdd-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e6cdd-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6cdd-135">Authorization</span></span> | <span data-ttu-id="e6cdd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e6cdd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cdd-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e6cdd-139">CSV</span><span class="sxs-lookup"><span data-stu-id="e6cdd-139">CSV</span></span>

<span data-ttu-id="e6cdd-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6cdd-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6cdd-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6cdd-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6cdd-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e6cdd-144">Report Refresh Date</span></span>
- <span data-ttu-id="e6cdd-145">Curtidos</span><span class="sxs-lookup"><span data-stu-id="e6cdd-145">Liked</span></span>
- <span data-ttu-id="e6cdd-146">Postados</span><span class="sxs-lookup"><span data-stu-id="e6cdd-146">Posted</span></span>
- <span data-ttu-id="e6cdd-147">Ler</span><span class="sxs-lookup"><span data-stu-id="e6cdd-147">Read</span></span>
- <span data-ttu-id="e6cdd-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e6cdd-148">Report Date</span></span>
- <span data-ttu-id="e6cdd-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e6cdd-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e6cdd-150">JSON</span><span class="sxs-lookup"><span data-stu-id="e6cdd-150">JSON</span></span>

<span data-ttu-id="e6cdd-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6cdd-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6cdd-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e6cdd-153">CSV</span><span class="sxs-lookup"><span data-stu-id="e6cdd-153">CSV</span></span>

<span data-ttu-id="e6cdd-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e6cdd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cdd-155">Request</span></span>

<span data-ttu-id="e6cdd-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e6cdd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cdd-157">Response</span></span>

<span data-ttu-id="e6cdd-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6cdd-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e6cdd-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6cdd-160">Basic</span><span class="sxs-lookup"><span data-stu-id="e6cdd-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6cdd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6cdd-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e6cdd-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e6cdd-163">JSON</span><span class="sxs-lookup"><span data-stu-id="e6cdd-163">JSON</span></span>

<span data-ttu-id="e6cdd-164">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e6cdd-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6cdd-165">Request</span></span>

<span data-ttu-id="e6cdd-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e6cdd-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6cdd-167">Response</span></span>

<span data-ttu-id="e6cdd-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-168">The following is an example of the response.</span></span>

> <span data-ttu-id="e6cdd-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6cdd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6cdd-171">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e6cdd-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6cdd-172">Basic</span><span class="sxs-lookup"><span data-stu-id="e6cdd-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6cdd-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6cdd-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
