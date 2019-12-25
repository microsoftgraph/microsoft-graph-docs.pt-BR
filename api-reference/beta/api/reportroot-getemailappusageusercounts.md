---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8d3e756cd7dd1fd03614e0b5cd93c5ad75cad85f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869238"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="ddac1-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ddac1-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddac1-104">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="ddac1-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="ddac1-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="ddac1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddac1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddac1-106">Permissions</span></span>

<span data-ttu-id="ddac1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddac1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddac1-109">Permission type</span></span>                        | <span data-ttu-id="ddac1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddac1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ddac1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddac1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddac1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddac1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ddac1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddac1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddac1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddac1-114">Not supported.</span></span>                           |
| <span data-ttu-id="ddac1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddac1-115">Application</span></span>                            | <span data-ttu-id="ddac1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddac1-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ddac1-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="ddac1-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ddac1-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ddac1-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ddac1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddac1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ddac1-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ddac1-120">Function parameters</span></span>

<span data-ttu-id="ddac1-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ddac1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ddac1-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ddac1-122">Parameter</span></span> | <span data-ttu-id="ddac1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddac1-123">Type</span></span>   | <span data-ttu-id="ddac1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddac1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ddac1-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ddac1-125">period</span></span>    | <span data-ttu-id="ddac1-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddac1-126">string</span></span> | <span data-ttu-id="ddac1-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ddac1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ddac1-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ddac1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ddac1-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ddac1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ddac1-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddac1-130">Required.</span></span> |

<span data-ttu-id="ddac1-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddac1-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ddac1-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="ddac1-132">The default output type is text/csv.</span></span> <span data-ttu-id="ddac1-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ddac1-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddac1-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddac1-134">Request headers</span></span>

| <span data-ttu-id="ddac1-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ddac1-135">Name</span></span>          | <span data-ttu-id="ddac1-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddac1-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ddac1-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddac1-137">Authorization</span></span> | <span data-ttu-id="ddac1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddac1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ddac1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddac1-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ddac1-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ddac1-141">CSV</span></span>

<span data-ttu-id="ddac1-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ddac1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ddac1-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ddac1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ddac1-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ddac1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ddac1-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ddac1-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ddac1-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ddac1-146">Report Refresh Date</span></span>
- <span data-ttu-id="ddac1-147">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="ddac1-147">Mail For Mac</span></span>
- <span data-ttu-id="ddac1-148">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="ddac1-148">Outlook For Mac</span></span>
- <span data-ttu-id="ddac1-149">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="ddac1-149">Outlook For Windows</span></span>
- <span data-ttu-id="ddac1-150">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="ddac1-150">Outlook For Mobile</span></span>
- <span data-ttu-id="ddac1-151">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="ddac1-151">Other For Mobile</span></span>
- <span data-ttu-id="ddac1-152">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="ddac1-152">Outlook For Web</span></span>
- <span data-ttu-id="ddac1-153">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="ddac1-153">POP3 App</span></span>
- <span data-ttu-id="ddac1-154">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="ddac1-154">IMAP4 App</span></span>
- <span data-ttu-id="ddac1-155">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="ddac1-155">SMTP App</span></span>
- <span data-ttu-id="ddac1-156">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ddac1-156">Report Date</span></span>
- <span data-ttu-id="ddac1-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ddac1-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ddac1-158">JSON</span><span class="sxs-lookup"><span data-stu-id="ddac1-158">JSON</span></span>

<span data-ttu-id="ddac1-159">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddac1-159">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddac1-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddac1-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ddac1-161">CSV</span><span class="sxs-lookup"><span data-stu-id="ddac1-161">CSV</span></span>

<span data-ttu-id="ddac1-162">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="ddac1-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ddac1-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddac1-163">Request</span></span>

<span data-ttu-id="ddac1-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddac1-164">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ddac1-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddac1-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddac1-166">C#</span><span class="sxs-lookup"><span data-stu-id="ddac1-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddac1-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddac1-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddac1-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddac1-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddac1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddac1-169">Response</span></span>

<span data-ttu-id="ddac1-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddac1-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ddac1-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ddac1-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ddac1-172">JSON</span><span class="sxs-lookup"><span data-stu-id="ddac1-172">JSON</span></span>

<span data-ttu-id="ddac1-173">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="ddac1-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ddac1-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddac1-174">Request</span></span>

<span data-ttu-id="ddac1-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddac1-175">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ddac1-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddac1-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ddac1-177">C#</span><span class="sxs-lookup"><span data-stu-id="ddac1-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ddac1-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddac1-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ddac1-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddac1-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ddac1-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddac1-180">Response</span></span>

<span data-ttu-id="ddac1-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddac1-181">The following is an example of the response.</span></span>

> <span data-ttu-id="ddac1-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddac1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
