---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 80a89e084bbdf8adb820015b68d2b6ef4d8b4bbb
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639513"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="ac800-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac800-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac800-104">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="ac800-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="ac800-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="ac800-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac800-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac800-106">Permissions</span></span>

<span data-ttu-id="ac800-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac800-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac800-109">Permission type</span></span>                        | <span data-ttu-id="ac800-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac800-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ac800-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac800-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac800-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac800-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ac800-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac800-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac800-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac800-114">Not supported.</span></span>                           |
| <span data-ttu-id="ac800-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac800-115">Application</span></span>                            | <span data-ttu-id="ac800-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac800-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ac800-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac800-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ac800-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ac800-118">Function parameters</span></span>

<span data-ttu-id="ac800-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ac800-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ac800-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ac800-120">Parameter</span></span> | <span data-ttu-id="ac800-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac800-121">Type</span></span>   | <span data-ttu-id="ac800-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac800-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ac800-123">ponto</span><span class="sxs-lookup"><span data-stu-id="ac800-123">period</span></span>    | <span data-ttu-id="ac800-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac800-124">string</span></span> | <span data-ttu-id="ac800-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ac800-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ac800-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ac800-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ac800-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ac800-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ac800-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac800-128">Required.</span></span> |

<span data-ttu-id="ac800-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac800-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ac800-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="ac800-130">The default output type is text/csv.</span></span> <span data-ttu-id="ac800-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ac800-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac800-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac800-132">Request headers</span></span>

| <span data-ttu-id="ac800-133">Nome</span><span class="sxs-lookup"><span data-stu-id="ac800-133">Name</span></span>          | <span data-ttu-id="ac800-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac800-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ac800-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac800-135">Authorization</span></span> | <span data-ttu-id="ac800-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac800-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ac800-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac800-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ac800-139">CSV</span><span class="sxs-lookup"><span data-stu-id="ac800-139">CSV</span></span>

<span data-ttu-id="ac800-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ac800-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ac800-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ac800-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ac800-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ac800-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ac800-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ac800-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ac800-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ac800-144">Report Refresh Date</span></span>
- <span data-ttu-id="ac800-145">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="ac800-145">Mail For Mac</span></span>
- <span data-ttu-id="ac800-146">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="ac800-146">Outlook For Mac</span></span>
- <span data-ttu-id="ac800-147">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="ac800-147">Outlook For Windows</span></span>
- <span data-ttu-id="ac800-148">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="ac800-148">Outlook For Mobile</span></span>
- <span data-ttu-id="ac800-149">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="ac800-149">Other For Mobile</span></span>
- <span data-ttu-id="ac800-150">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="ac800-150">Outlook For Web</span></span>
- <span data-ttu-id="ac800-151">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="ac800-151">POP3 App</span></span>
- <span data-ttu-id="ac800-152">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="ac800-152">IMAP4 App</span></span>
- <span data-ttu-id="ac800-153">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="ac800-153">SMTP App</span></span>
- <span data-ttu-id="ac800-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ac800-154">Report Date</span></span>
- <span data-ttu-id="ac800-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ac800-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ac800-156">JSON</span><span class="sxs-lookup"><span data-stu-id="ac800-156">JSON</span></span>

<span data-ttu-id="ac800-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac800-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac800-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac800-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ac800-159">CSV</span><span class="sxs-lookup"><span data-stu-id="ac800-159">CSV</span></span>

<span data-ttu-id="ac800-160">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="ac800-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ac800-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac800-161">Request</span></span>

<span data-ttu-id="ac800-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac800-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ac800-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac800-163">Response</span></span>

<span data-ttu-id="ac800-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac800-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ac800-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ac800-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ac800-166">Basic</span><span class="sxs-lookup"><span data-stu-id="ac800-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac800-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac800-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ac800-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ac800-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ac800-169">JSON</span><span class="sxs-lookup"><span data-stu-id="ac800-169">JSON</span></span>

<span data-ttu-id="ac800-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="ac800-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ac800-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac800-171">Request</span></span>

<span data-ttu-id="ac800-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac800-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ac800-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac800-173">Response</span></span>

<span data-ttu-id="ac800-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac800-174">The following is an example of the response.</span></span>

> <span data-ttu-id="ac800-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac800-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ac800-177">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ac800-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ac800-178">Basic</span><span class="sxs-lookup"><span data-stu-id="ac800-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac800-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac800-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
