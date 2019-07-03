---
title: 'reportRoot: getEmailActivityCounts'
description: Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: abf0f0624cfc41124f03bd3f5872054cadc2c4a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447107"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="8edbd-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="8edbd-103">reportRoot: getEmailActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8edbd-104">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="8edbd-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="8edbd-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="8edbd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="8edbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8edbd-106">Permissions</span></span>

<span data-ttu-id="8edbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8edbd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8edbd-109">Permission type</span></span>                        | <span data-ttu-id="8edbd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8edbd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8edbd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8edbd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8edbd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edbd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8edbd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8edbd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8edbd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8edbd-114">Not supported.</span></span>                           |
| <span data-ttu-id="8edbd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8edbd-115">Application</span></span>                            | <span data-ttu-id="8edbd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edbd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8edbd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8edbd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8edbd-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8edbd-118">Function parameters</span></span>

<span data-ttu-id="8edbd-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8edbd-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8edbd-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8edbd-120">Parameter</span></span> | <span data-ttu-id="8edbd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8edbd-121">Type</span></span>   | <span data-ttu-id="8edbd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8edbd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8edbd-123">ponto</span><span class="sxs-lookup"><span data-stu-id="8edbd-123">period</span></span>    | <span data-ttu-id="8edbd-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8edbd-124">string</span></span> | <span data-ttu-id="8edbd-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8edbd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8edbd-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8edbd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8edbd-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8edbd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8edbd-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8edbd-128">Required.</span></span> |

<span data-ttu-id="8edbd-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8edbd-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8edbd-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="8edbd-130">The default output type is text/csv.</span></span> <span data-ttu-id="8edbd-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8edbd-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8edbd-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8edbd-132">Request headers</span></span>

| <span data-ttu-id="8edbd-133">Nome</span><span class="sxs-lookup"><span data-stu-id="8edbd-133">Name</span></span>          | <span data-ttu-id="8edbd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8edbd-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8edbd-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="8edbd-135">Authorization</span></span> | <span data-ttu-id="8edbd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8edbd-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8edbd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edbd-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8edbd-139">CSV</span><span class="sxs-lookup"><span data-stu-id="8edbd-139">CSV</span></span>

<span data-ttu-id="8edbd-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8edbd-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8edbd-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8edbd-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8edbd-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8edbd-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8edbd-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8edbd-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8edbd-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8edbd-144">Report Refresh Date</span></span>
- <span data-ttu-id="8edbd-145">Enviar</span><span class="sxs-lookup"><span data-stu-id="8edbd-145">Send</span></span>
- <span data-ttu-id="8edbd-146">Receber</span><span class="sxs-lookup"><span data-stu-id="8edbd-146">Receive</span></span>
- <span data-ttu-id="8edbd-147">Ler</span><span class="sxs-lookup"><span data-stu-id="8edbd-147">Read</span></span>
- <span data-ttu-id="8edbd-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="8edbd-148">Report Date</span></span>
- <span data-ttu-id="8edbd-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8edbd-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8edbd-150">JSON</span><span class="sxs-lookup"><span data-stu-id="8edbd-150">JSON</span></span>

<span data-ttu-id="8edbd-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailActivitySummary](../resources/emailactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8edbd-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8edbd-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8edbd-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8edbd-153">CSV</span><span class="sxs-lookup"><span data-stu-id="8edbd-153">CSV</span></span>

<span data-ttu-id="8edbd-154">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="8edbd-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8edbd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8edbd-155">Request</span></span>

<span data-ttu-id="8edbd-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8edbd-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8edbd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8edbd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8edbd-158">C#</span><span class="sxs-lookup"><span data-stu-id="8edbd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8edbd-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="8edbd-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8edbd-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8edbd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8edbd-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edbd-161">Response</span></span>

<span data-ttu-id="8edbd-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8edbd-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8edbd-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8edbd-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="8edbd-164">JSON</span><span class="sxs-lookup"><span data-stu-id="8edbd-164">JSON</span></span>

<span data-ttu-id="8edbd-165">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="8edbd-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8edbd-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8edbd-166">Request</span></span>

<span data-ttu-id="8edbd-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8edbd-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8edbd-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="8edbd-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8edbd-169">C#</span><span class="sxs-lookup"><span data-stu-id="8edbd-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8edbd-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="8edbd-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8edbd-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8edbd-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8edbd-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8edbd-172">Response</span></span>

<span data-ttu-id="8edbd-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8edbd-173">The following is an example of the response.</span></span>

> <span data-ttu-id="8edbd-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8edbd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
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
