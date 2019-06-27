---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4fe68eca6dc0c5a5fbc60953eea2fbf6493384df
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267946"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="f2539-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f2539-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2539-104">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="f2539-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="f2539-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="f2539-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2539-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2539-106">Permissions</span></span>

<span data-ttu-id="f2539-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2539-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2539-109">Permission type</span></span>                        | <span data-ttu-id="f2539-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2539-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f2539-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2539-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2539-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2539-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f2539-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2539-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2539-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2539-114">Not supported.</span></span>                           |
| <span data-ttu-id="f2539-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2539-115">Application</span></span>                            | <span data-ttu-id="f2539-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2539-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f2539-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2539-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="f2539-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f2539-118">Function parameters</span></span>

<span data-ttu-id="f2539-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f2539-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="f2539-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2539-120">Parameter</span></span> | <span data-ttu-id="f2539-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2539-121">Type</span></span>   | <span data-ttu-id="f2539-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2539-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f2539-123">ponto</span><span class="sxs-lookup"><span data-stu-id="f2539-123">period</span></span>    | <span data-ttu-id="f2539-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2539-124">string</span></span> | <span data-ttu-id="f2539-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f2539-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f2539-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f2539-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f2539-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f2539-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="f2539-128">data</span><span class="sxs-lookup"><span data-stu-id="f2539-128">date</span></span>      | <span data-ttu-id="f2539-129">Data</span><span class="sxs-lookup"><span data-stu-id="f2539-129">Date</span></span>   | <span data-ttu-id="f2539-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="f2539-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="f2539-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="f2539-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="f2539-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="f2539-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="f2539-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="f2539-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="f2539-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="f2539-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f2539-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="f2539-135">The default output type is text/csv.</span></span> <span data-ttu-id="f2539-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="f2539-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2539-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2539-137">Request headers</span></span>

| <span data-ttu-id="f2539-138">Nome</span><span class="sxs-lookup"><span data-stu-id="f2539-138">Name</span></span>          | <span data-ttu-id="f2539-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2539-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f2539-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2539-140">Authorization</span></span> | <span data-ttu-id="f2539-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2539-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f2539-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2539-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f2539-144">CSV</span><span class="sxs-lookup"><span data-stu-id="f2539-144">CSV</span></span>

<span data-ttu-id="f2539-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f2539-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f2539-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f2539-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f2539-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f2539-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f2539-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f2539-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f2539-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f2539-149">Report Refresh Date</span></span>
- <span data-ttu-id="f2539-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="f2539-150">User Principal Name</span></span>
- <span data-ttu-id="f2539-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f2539-151">Display Name</span></span>
- <span data-ttu-id="f2539-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="f2539-152">Is Deleted</span></span>
- <span data-ttu-id="f2539-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="f2539-153">Deleted Date</span></span>
- <span data-ttu-id="f2539-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="f2539-154">Last Activity Date</span></span>
- <span data-ttu-id="f2539-155">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="f2539-155">Mail For Mac</span></span>
- <span data-ttu-id="f2539-156">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="f2539-156">Outlook For Mac</span></span>
- <span data-ttu-id="f2539-157">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="f2539-157">Outlook For Windows</span></span>
- <span data-ttu-id="f2539-158">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="f2539-158">Outlook For Mobile</span></span>
- <span data-ttu-id="f2539-159">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="f2539-159">Other For Mobile</span></span>
- <span data-ttu-id="f2539-160">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="f2539-160">Outlook For Web</span></span>
- <span data-ttu-id="f2539-161">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="f2539-161">POP3 App</span></span>
- <span data-ttu-id="f2539-162">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="f2539-162">IMAP4 App</span></span>
- <span data-ttu-id="f2539-163">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="f2539-163">SMTP App</span></span>
- <span data-ttu-id="f2539-164">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f2539-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f2539-165">JSON</span><span class="sxs-lookup"><span data-stu-id="f2539-165">JSON</span></span>

<span data-ttu-id="f2539-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2539-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="f2539-167">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="f2539-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="f2539-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2539-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f2539-169">CSV</span><span class="sxs-lookup"><span data-stu-id="f2539-169">CSV</span></span>

<span data-ttu-id="f2539-170">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="f2539-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f2539-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2539-171">Request</span></span>

<span data-ttu-id="f2539-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2539-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="f2539-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2539-173">Response</span></span>

<span data-ttu-id="f2539-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2539-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2539-175">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="f2539-175">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2539-176">C#</span><span class="sxs-lookup"><span data-stu-id="f2539-176">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2539-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2539-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f2539-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f2539-178">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="f2539-179">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f2539-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="f2539-180">JSON</span><span class="sxs-lookup"><span data-stu-id="f2539-180">JSON</span></span>

<span data-ttu-id="f2539-181">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="f2539-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f2539-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2539-182">Request</span></span>

<span data-ttu-id="f2539-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2539-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="f2539-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2539-184">Response</span></span>

<span data-ttu-id="f2539-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2539-185">The following is an example of the response.</span></span>

> <span data-ttu-id="f2539-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2539-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2539-188">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f2539-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2539-189">C#</span><span class="sxs-lookup"><span data-stu-id="f2539-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2539-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2539-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f2539-191">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f2539-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageuserdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
