---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 6baa9d72cb6f25474a3d377065f8df2daa9dd414
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639534"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="bfb6b-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="bfb6b-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb6b-104">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="bfb6b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="bfb6b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb6b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfb6b-106">Permissions</span></span>

<span data-ttu-id="bfb6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfb6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfb6b-109">Permission type</span></span>                        | <span data-ttu-id="bfb6b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfb6b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bfb6b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfb6b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfb6b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfb6b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bfb6b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfb6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb6b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-114">Not supported.</span></span>                           |
| <span data-ttu-id="bfb6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfb6b-115">Application</span></span>                            | <span data-ttu-id="bfb6b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfb6b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bfb6b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb6b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bfb6b-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bfb6b-118">Function parameters</span></span>

<span data-ttu-id="bfb6b-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bfb6b-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bfb6b-120">Parameter</span></span> | <span data-ttu-id="bfb6b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfb6b-121">Type</span></span>   | <span data-ttu-id="bfb6b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb6b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bfb6b-123">ponto</span><span class="sxs-lookup"><span data-stu-id="bfb6b-123">period</span></span>    | <span data-ttu-id="bfb6b-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfb6b-124">string</span></span> | <span data-ttu-id="bfb6b-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bfb6b-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bfb6b-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bfb6b-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-128">Required.</span></span> |

<span data-ttu-id="bfb6b-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bfb6b-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-130">The default output type is text/csv.</span></span> <span data-ttu-id="bfb6b-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfb6b-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb6b-132">Request headers</span></span>

| <span data-ttu-id="bfb6b-133">Nome</span><span class="sxs-lookup"><span data-stu-id="bfb6b-133">Name</span></span>          | <span data-ttu-id="bfb6b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb6b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bfb6b-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfb6b-135">Authorization</span></span> | <span data-ttu-id="bfb6b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bfb6b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb6b-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bfb6b-139">CSV</span><span class="sxs-lookup"><span data-stu-id="bfb6b-139">CSV</span></span>

<span data-ttu-id="bfb6b-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bfb6b-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bfb6b-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bfb6b-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bfb6b-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bfb6b-144">Report Refresh Date</span></span>
- <span data-ttu-id="bfb6b-145">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="bfb6b-145">Mail For Mac</span></span>
- <span data-ttu-id="bfb6b-146">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="bfb6b-146">Outlook For Mac</span></span>
- <span data-ttu-id="bfb6b-147">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="bfb6b-147">Outlook For Windows</span></span>
- <span data-ttu-id="bfb6b-148">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="bfb6b-148">Outlook For Mobile</span></span>
- <span data-ttu-id="bfb6b-149">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="bfb6b-149">Other For Mobile</span></span>
- <span data-ttu-id="bfb6b-150">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="bfb6b-150">Outlook For Web</span></span>
- <span data-ttu-id="bfb6b-151">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="bfb6b-151">POP3 App</span></span>
- <span data-ttu-id="bfb6b-152">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="bfb6b-152">IMAP4 App</span></span>
- <span data-ttu-id="bfb6b-153">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="bfb6b-153">SMTP App</span></span>
- <span data-ttu-id="bfb6b-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bfb6b-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bfb6b-155">JSON</span><span class="sxs-lookup"><span data-stu-id="bfb6b-155">JSON</span></span>

<span data-ttu-id="bfb6b-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-156">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfb6b-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfb6b-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bfb6b-158">CSV</span><span class="sxs-lookup"><span data-stu-id="bfb6b-158">CSV</span></span>

<span data-ttu-id="bfb6b-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bfb6b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb6b-160">Request</span></span>

<span data-ttu-id="bfb6b-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bfb6b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb6b-162">Response</span></span>

<span data-ttu-id="bfb6b-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bfb6b-164">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bfb6b-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bfb6b-165">Basic</span><span class="sxs-lookup"><span data-stu-id="bfb6b-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageappsusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfb6b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb6b-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageappsusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bfb6b-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="bfb6b-168">JSON</span><span class="sxs-lookup"><span data-stu-id="bfb6b-168">JSON</span></span>

<span data-ttu-id="bfb6b-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bfb6b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb6b-170">Request</span></span>

<span data-ttu-id="bfb6b-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bfb6b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb6b-172">Response</span></span>

<span data-ttu-id="bfb6b-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-173">The following is an example of the response.</span></span>

> <span data-ttu-id="bfb6b-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfb6b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bfb6b-176">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bfb6b-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bfb6b-177">Basic</span><span class="sxs-lookup"><span data-stu-id="bfb6b-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageappsusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfb6b-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb6b-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageappsusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getemailappusageappsusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageappsusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageappsusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageappsusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
