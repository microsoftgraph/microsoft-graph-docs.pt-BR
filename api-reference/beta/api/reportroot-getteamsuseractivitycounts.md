---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9419d718da821a012b74db8ed37529ca843bb5c4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871713"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="36937-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="36937-104">reportRoot: getTeamsUserActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36937-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="36937-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="36937-106">Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="36937-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="36937-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="36937-107">Permissions</span></span>

<span data-ttu-id="36937-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36937-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36937-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36937-110">Permission type</span></span>                        | <span data-ttu-id="36937-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36937-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="36937-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36937-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="36937-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36937-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="36937-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36937-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36937-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36937-115">Not supported.</span></span>                           |
| <span data-ttu-id="36937-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36937-116">Application</span></span>                            | <span data-ttu-id="36937-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="36937-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="36937-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36937-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="36937-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="36937-119">Function parameters</span></span>

<span data-ttu-id="36937-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="36937-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="36937-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="36937-121">Parameter</span></span> | <span data-ttu-id="36937-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="36937-122">Type</span></span>   | <span data-ttu-id="36937-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="36937-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="36937-124">ponto</span><span class="sxs-lookup"><span data-stu-id="36937-124">period</span></span>    | <span data-ttu-id="36937-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36937-125">string</span></span> | <span data-ttu-id="36937-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="36937-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="36937-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="36937-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="36937-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="36937-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="36937-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36937-129">Required.</span></span> |

<span data-ttu-id="36937-130">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36937-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="36937-131">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="36937-131">The default output type is text/csv.</span></span> <span data-ttu-id="36937-132">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="36937-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36937-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36937-133">Request headers</span></span>

| <span data-ttu-id="36937-134">Nome</span><span class="sxs-lookup"><span data-stu-id="36937-134">Name</span></span>          | <span data-ttu-id="36937-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="36937-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="36937-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="36937-136">Authorization</span></span> | <span data-ttu-id="36937-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36937-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="36937-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="36937-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="36937-140">CSV</span><span class="sxs-lookup"><span data-stu-id="36937-140">CSV</span></span>

<span data-ttu-id="36937-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="36937-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="36937-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="36937-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="36937-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="36937-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="36937-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="36937-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="36937-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="36937-145">Report Refresh Date</span></span>
- <span data-ttu-id="36937-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="36937-146">Report Date</span></span>
- <span data-ttu-id="36937-147">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="36937-147">Team Chat Messages</span></span>
- <span data-ttu-id="36937-148">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="36937-148">Private Chat Messages</span></span>
- <span data-ttu-id="36937-149">Chamadas</span><span class="sxs-lookup"><span data-stu-id="36937-149">Calls</span></span>
- <span data-ttu-id="36937-150">Reuniões</span><span class="sxs-lookup"><span data-stu-id="36937-150">Meetings</span></span>
- <span data-ttu-id="36937-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="36937-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="36937-152">JSON</span><span class="sxs-lookup"><span data-stu-id="36937-152">JSON</span></span>

<span data-ttu-id="36937-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36937-153">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36937-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36937-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="36937-155">CSV</span><span class="sxs-lookup"><span data-stu-id="36937-155">CSV</span></span>

<span data-ttu-id="36937-156">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="36937-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="36937-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36937-157">Request</span></span>

<span data-ttu-id="36937-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36937-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36937-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="36937-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36937-160">C#</span><span class="sxs-lookup"><span data-stu-id="36937-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36937-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="36937-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36937-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="36937-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36937-163">Java</span><span class="sxs-lookup"><span data-stu-id="36937-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36937-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="36937-164">Response</span></span>

<span data-ttu-id="36937-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36937-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="36937-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="36937-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="36937-167">JSON</span><span class="sxs-lookup"><span data-stu-id="36937-167">JSON</span></span>

<span data-ttu-id="36937-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="36937-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="36937-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36937-169">Request</span></span>

<span data-ttu-id="36937-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36937-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36937-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="36937-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36937-172">C#</span><span class="sxs-lookup"><span data-stu-id="36937-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36937-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="36937-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36937-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="36937-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36937-175">Java</span><span class="sxs-lookup"><span data-stu-id="36937-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36937-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="36937-176">Response</span></span>

<span data-ttu-id="36937-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36937-177">The following is an example of the response.</span></span>

> <span data-ttu-id="36937-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36937-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
