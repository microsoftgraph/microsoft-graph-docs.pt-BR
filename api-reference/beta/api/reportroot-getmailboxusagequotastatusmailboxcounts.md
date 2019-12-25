---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 587ffd19690f4e6264b250c1b3e1602085bec773
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869187"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="e7159-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e7159-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7159-104">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="e7159-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="e7159-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e7159-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7159-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7159-106">Permissions</span></span>

<span data-ttu-id="e7159-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7159-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7159-109">Permission type</span></span>                        | <span data-ttu-id="e7159-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7159-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e7159-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7159-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7159-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7159-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e7159-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7159-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7159-114">Not supported.</span></span>                           |
| <span data-ttu-id="e7159-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7159-115">Application</span></span>                            | <span data-ttu-id="e7159-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7159-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="e7159-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="e7159-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e7159-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e7159-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e7159-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7159-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e7159-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e7159-120">Function parameters</span></span>

<span data-ttu-id="e7159-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e7159-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e7159-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e7159-122">Parameter</span></span> | <span data-ttu-id="e7159-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7159-123">Type</span></span>   | <span data-ttu-id="e7159-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7159-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e7159-125">ponto</span><span class="sxs-lookup"><span data-stu-id="e7159-125">period</span></span>    | <span data-ttu-id="e7159-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7159-126">string</span></span> | <span data-ttu-id="e7159-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e7159-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e7159-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e7159-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e7159-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e7159-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e7159-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7159-130">Required.</span></span> |

<span data-ttu-id="e7159-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e7159-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e7159-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="e7159-132">The default output type is text/csv.</span></span> <span data-ttu-id="e7159-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e7159-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7159-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7159-134">Request headers</span></span>

| <span data-ttu-id="e7159-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e7159-135">Name</span></span>          | <span data-ttu-id="e7159-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7159-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e7159-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7159-137">Authorization</span></span> | <span data-ttu-id="e7159-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7159-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e7159-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7159-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e7159-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e7159-141">CSV</span></span>

<span data-ttu-id="e7159-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e7159-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e7159-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e7159-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e7159-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e7159-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e7159-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e7159-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e7159-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e7159-146">Report Refresh Date</span></span>
- <span data-ttu-id="e7159-147">Abaixo do limite</span><span class="sxs-lookup"><span data-stu-id="e7159-147">Under Limit</span></span>
- <span data-ttu-id="e7159-148">Aviso emitido</span><span class="sxs-lookup"><span data-stu-id="e7159-148">Warning Issued</span></span>
- <span data-ttu-id="e7159-149">Envio proibido</span><span class="sxs-lookup"><span data-stu-id="e7159-149">Send Prohibited</span></span>
- <span data-ttu-id="e7159-150">Envio/recebimento proibido</span><span class="sxs-lookup"><span data-stu-id="e7159-150">Send/Receive Prohibited</span></span>
- <span data-ttu-id="e7159-151">Indeterminado</span><span class="sxs-lookup"><span data-stu-id="e7159-151">Indeterminate</span></span>
- <span data-ttu-id="e7159-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e7159-152">Report Date</span></span>
- <span data-ttu-id="e7159-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e7159-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e7159-154">JSON</span><span class="sxs-lookup"><span data-stu-id="e7159-154">JSON</span></span>

<span data-ttu-id="e7159-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7159-155">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7159-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7159-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e7159-157">CSV</span><span class="sxs-lookup"><span data-stu-id="e7159-157">CSV</span></span>

<span data-ttu-id="e7159-158">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="e7159-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e7159-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7159-159">Request</span></span>

<span data-ttu-id="e7159-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7159-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7159-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7159-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7159-162">C#</span><span class="sxs-lookup"><span data-stu-id="e7159-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7159-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7159-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7159-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7159-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7159-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7159-165">Response</span></span>

<span data-ttu-id="e7159-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7159-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e7159-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e7159-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e7159-168">JSON</span><span class="sxs-lookup"><span data-stu-id="e7159-168">JSON</span></span>

<span data-ttu-id="e7159-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e7159-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e7159-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7159-170">Request</span></span>

<span data-ttu-id="e7159-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7159-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e7159-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7159-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7159-173">C#</span><span class="sxs-lookup"><span data-stu-id="e7159-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7159-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7159-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7159-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7159-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e7159-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7159-176">Response</span></span>

<span data-ttu-id="e7159-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7159-177">The following is an example of the response.</span></span>

> <span data-ttu-id="e7159-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7159-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageQuotaMailboxStatusCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "underLimit": 155, 
      "warningIssued": 0, 
      "sendProhibited": 0, 
      "sendReceiveProhibited": 0, 
      "indeterminate": 14, 
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
