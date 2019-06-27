---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 80afd380f12c7a128c6f3066c6db2df87168f9fa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269087"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="6a8ea-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="6a8ea-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a8ea-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="6a8ea-106">Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a8ea-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a8ea-107">Permissions</span></span>

<span data-ttu-id="6a8ea-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a8ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a8ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a8ea-110">Permission type</span></span>                        | <span data-ttu-id="6a8ea-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a8ea-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6a8ea-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a8ea-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a8ea-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a8ea-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6a8ea-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a8ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-115">Not supported.</span></span>                           |
| <span data-ttu-id="6a8ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a8ea-116">Application</span></span>                            | <span data-ttu-id="6a8ea-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a8ea-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6a8ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a8ea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="6a8ea-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6a8ea-119">Function parameters</span></span>

<span data-ttu-id="6a8ea-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6a8ea-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6a8ea-121">Parameter</span></span> | <span data-ttu-id="6a8ea-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a8ea-122">Type</span></span>   | <span data-ttu-id="6a8ea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a8ea-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6a8ea-124">ponto</span><span class="sxs-lookup"><span data-stu-id="6a8ea-124">period</span></span>    | <span data-ttu-id="6a8ea-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a8ea-125">string</span></span> | <span data-ttu-id="6a8ea-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6a8ea-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6a8ea-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6a8ea-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-129">Required.</span></span> |

<span data-ttu-id="6a8ea-130">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6a8ea-131">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-131">The default output type is text/csv.</span></span> <span data-ttu-id="6a8ea-132">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a8ea-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8ea-133">Request headers</span></span>

| <span data-ttu-id="6a8ea-134">Nome</span><span class="sxs-lookup"><span data-stu-id="6a8ea-134">Name</span></span>          | <span data-ttu-id="6a8ea-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a8ea-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6a8ea-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a8ea-136">Authorization</span></span> | <span data-ttu-id="6a8ea-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6a8ea-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8ea-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6a8ea-140">CSV</span><span class="sxs-lookup"><span data-stu-id="6a8ea-140">CSV</span></span>

<span data-ttu-id="6a8ea-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6a8ea-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6a8ea-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6a8ea-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6a8ea-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6a8ea-145">Report Refresh Date</span></span>
- <span data-ttu-id="6a8ea-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6a8ea-146">Report Date</span></span>
- <span data-ttu-id="6a8ea-147">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="6a8ea-147">Team Chat Messages</span></span>
- <span data-ttu-id="6a8ea-148">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="6a8ea-148">Private Chat Messages</span></span>
- <span data-ttu-id="6a8ea-149">Chamadas</span><span class="sxs-lookup"><span data-stu-id="6a8ea-149">Calls</span></span>
- <span data-ttu-id="6a8ea-150">Reuniões</span><span class="sxs-lookup"><span data-stu-id="6a8ea-150">Meetings</span></span>
- <span data-ttu-id="6a8ea-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6a8ea-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6a8ea-152">JSON</span><span class="sxs-lookup"><span data-stu-id="6a8ea-152">JSON</span></span>

<span data-ttu-id="6a8ea-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a8ea-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a8ea-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6a8ea-155">CSV</span><span class="sxs-lookup"><span data-stu-id="6a8ea-155">CSV</span></span>

<span data-ttu-id="6a8ea-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6a8ea-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8ea-157">Request</span></span>

<span data-ttu-id="6a8ea-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6a8ea-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8ea-159">Response</span></span>

<span data-ttu-id="6a8ea-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a8ea-161">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="6a8ea-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a8ea-162">C#</span><span class="sxs-lookup"><span data-stu-id="6a8ea-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a8ea-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a8ea-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6a8ea-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a8ea-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<span data-ttu-id="6a8ea-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="6a8ea-166">JSON</span><span class="sxs-lookup"><span data-stu-id="6a8ea-166">JSON</span></span>

<span data-ttu-id="6a8ea-167">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6a8ea-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a8ea-168">Request</span></span>

<span data-ttu-id="6a8ea-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6a8ea-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a8ea-170">Response</span></span>

<span data-ttu-id="6a8ea-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-171">The following is an example of the response.</span></span>

> <span data-ttu-id="6a8ea-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a8ea-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a8ea-174">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6a8ea-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a8ea-175">C#</span><span class="sxs-lookup"><span data-stu-id="6a8ea-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a8ea-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a8ea-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6a8ea-177">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a8ea-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivitycounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
