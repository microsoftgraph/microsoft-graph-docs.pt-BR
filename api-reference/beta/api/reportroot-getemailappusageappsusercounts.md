---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4b221b03a816491c9591aecba0a9582ec8173565
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411862"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="4c728-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="4c728-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c728-104">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="4c728-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="4c728-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="4c728-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c728-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c728-106">Permissions</span></span>

<span data-ttu-id="4c728-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c728-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c728-109">Permission type</span></span>                        | <span data-ttu-id="4c728-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c728-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c728-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c728-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c728-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c728-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c728-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c728-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c728-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c728-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c728-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c728-115">Application</span></span>                            | <span data-ttu-id="4c728-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c728-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c728-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c728-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c728-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4c728-118">Function parameters</span></span>

<span data-ttu-id="4c728-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4c728-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c728-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c728-120">Parameter</span></span> | <span data-ttu-id="4c728-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c728-121">Type</span></span>   | <span data-ttu-id="4c728-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c728-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c728-123">ponto</span><span class="sxs-lookup"><span data-stu-id="4c728-123">period</span></span>    | <span data-ttu-id="4c728-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c728-124">string</span></span> | <span data-ttu-id="4c728-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c728-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c728-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4c728-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c728-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c728-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c728-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c728-128">Required.</span></span> |

<span data-ttu-id="4c728-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c728-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4c728-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="4c728-130">The default output type is text/csv.</span></span> <span data-ttu-id="4c728-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4c728-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c728-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c728-132">Request headers</span></span>

| <span data-ttu-id="4c728-133">Nome</span><span class="sxs-lookup"><span data-stu-id="4c728-133">Name</span></span>          | <span data-ttu-id="4c728-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c728-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4c728-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c728-135">Authorization</span></span> | <span data-ttu-id="4c728-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c728-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c728-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c728-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4c728-139">CSV</span><span class="sxs-lookup"><span data-stu-id="4c728-139">CSV</span></span>

<span data-ttu-id="4c728-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4c728-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c728-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4c728-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c728-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c728-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c728-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4c728-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c728-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4c728-144">Report Refresh Date</span></span>
- <span data-ttu-id="4c728-145">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="4c728-145">Mail For Mac</span></span>
- <span data-ttu-id="4c728-146">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="4c728-146">Outlook For Mac</span></span>
- <span data-ttu-id="4c728-147">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="4c728-147">Outlook For Windows</span></span>
- <span data-ttu-id="4c728-148">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="4c728-148">Outlook For Mobile</span></span>
- <span data-ttu-id="4c728-149">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="4c728-149">Other For Mobile</span></span>
- <span data-ttu-id="4c728-150">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="4c728-150">Outlook For Web</span></span>
- <span data-ttu-id="4c728-151">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="4c728-151">POP3 App</span></span>
- <span data-ttu-id="4c728-152">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="4c728-152">IMAP4 App</span></span>
- <span data-ttu-id="4c728-153">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="4c728-153">SMTP App</span></span>
- <span data-ttu-id="4c728-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4c728-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4c728-155">JSON</span><span class="sxs-lookup"><span data-stu-id="4c728-155">JSON</span></span>

<span data-ttu-id="4c728-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c728-156">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c728-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c728-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4c728-158">CSV</span><span class="sxs-lookup"><span data-stu-id="4c728-158">CSV</span></span>

<span data-ttu-id="4c728-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="4c728-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4c728-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c728-160">Request</span></span>

<span data-ttu-id="4c728-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c728-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c728-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c728-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c728-163">C#</span><span class="sxs-lookup"><span data-stu-id="4c728-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageappsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c728-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c728-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageappsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c728-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4c728-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageappsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c728-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c728-166">Response</span></span>

<span data-ttu-id="4c728-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c728-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4c728-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4c728-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="4c728-169">JSON</span><span class="sxs-lookup"><span data-stu-id="4c728-169">JSON</span></span>

<span data-ttu-id="4c728-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4c728-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4c728-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c728-171">Request</span></span>

<span data-ttu-id="4c728-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c728-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c728-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c728-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c728-174">C#</span><span class="sxs-lookup"><span data-stu-id="4c728-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageappsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c728-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c728-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageappsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c728-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4c728-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageappsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c728-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c728-177">Response</span></span>

<span data-ttu-id="4c728-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c728-178">The following is an example of the response.</span></span>

> <span data-ttu-id="4c728-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c728-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageAppsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 4, 
      "outlookForMac": 105, 
      "outlookForWindows": 1589, 
      "outlookForMobile": 1116, 
      "otherForMobile": 485, 
      "outlookForWeb": 753, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
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
