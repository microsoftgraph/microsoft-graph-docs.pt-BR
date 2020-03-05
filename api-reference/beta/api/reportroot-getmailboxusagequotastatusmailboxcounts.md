---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3f818779580b9c5a25ec93ba4fec2e034dc26d40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454414"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="1b6d6-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="1b6d6-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="1b6d6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1b6d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b6d6-105">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-105">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="1b6d6-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="1b6d6-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b6d6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b6d6-107">Permissions</span></span>

<span data-ttu-id="1b6d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b6d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b6d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b6d6-110">Permission type</span></span>                        | <span data-ttu-id="1b6d6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b6d6-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1b6d6-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b6d6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b6d6-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b6d6-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1b6d6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b6d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b6d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-115">Not supported.</span></span>                           |
| <span data-ttu-id="1b6d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b6d6-116">Application</span></span>                            | <span data-ttu-id="1b6d6-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b6d6-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="1b6d6-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1b6d6-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1b6d6-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b6d6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6d6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1b6d6-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1b6d6-121">Function parameters</span></span>

<span data-ttu-id="1b6d6-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1b6d6-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1b6d6-123">Parameter</span></span> | <span data-ttu-id="1b6d6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b6d6-124">Type</span></span>   | <span data-ttu-id="1b6d6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b6d6-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1b6d6-126">ponto</span><span class="sxs-lookup"><span data-stu-id="1b6d6-126">period</span></span>    | <span data-ttu-id="1b6d6-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b6d6-127">string</span></span> | <span data-ttu-id="1b6d6-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1b6d6-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1b6d6-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1b6d6-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-131">Required.</span></span> |

<span data-ttu-id="1b6d6-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1b6d6-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-133">The default output type is text/csv.</span></span> <span data-ttu-id="1b6d6-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b6d6-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6d6-135">Request headers</span></span>

| <span data-ttu-id="1b6d6-136">Nome</span><span class="sxs-lookup"><span data-stu-id="1b6d6-136">Name</span></span>          | <span data-ttu-id="1b6d6-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b6d6-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1b6d6-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b6d6-138">Authorization</span></span> | <span data-ttu-id="1b6d6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1b6d6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6d6-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1b6d6-142">CSV</span><span class="sxs-lookup"><span data-stu-id="1b6d6-142">CSV</span></span>

<span data-ttu-id="1b6d6-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1b6d6-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1b6d6-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1b6d6-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1b6d6-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1b6d6-147">Report Refresh Date</span></span>
- <span data-ttu-id="1b6d6-148">Abaixo do limite</span><span class="sxs-lookup"><span data-stu-id="1b6d6-148">Under Limit</span></span>
- <span data-ttu-id="1b6d6-149">Aviso emitido</span><span class="sxs-lookup"><span data-stu-id="1b6d6-149">Warning Issued</span></span>
- <span data-ttu-id="1b6d6-150">Envio proibido</span><span class="sxs-lookup"><span data-stu-id="1b6d6-150">Send Prohibited</span></span>
- <span data-ttu-id="1b6d6-151">Envio/recebimento proibido</span><span class="sxs-lookup"><span data-stu-id="1b6d6-151">Send/Receive Prohibited</span></span>
- <span data-ttu-id="1b6d6-152">Indeterminado</span><span class="sxs-lookup"><span data-stu-id="1b6d6-152">Indeterminate</span></span>
- <span data-ttu-id="1b6d6-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1b6d6-153">Report Date</span></span>
- <span data-ttu-id="1b6d6-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1b6d6-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1b6d6-155">JSON</span><span class="sxs-lookup"><span data-stu-id="1b6d6-155">JSON</span></span>

<span data-ttu-id="1b6d6-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-156">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b6d6-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b6d6-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1b6d6-158">CSV</span><span class="sxs-lookup"><span data-stu-id="1b6d6-158">CSV</span></span>

<span data-ttu-id="1b6d6-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1b6d6-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6d6-160">Request</span></span>

<span data-ttu-id="1b6d6-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b6d6-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6d6-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="1b6d6-163">C#</span><span class="sxs-lookup"><span data-stu-id="1b6d6-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b6d6-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b6d6-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b6d6-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b6d6-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b6d6-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6d6-166">Response</span></span>

<span data-ttu-id="1b6d6-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1b6d6-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1b6d6-169">JSON</span><span class="sxs-lookup"><span data-stu-id="1b6d6-169">JSON</span></span>

<span data-ttu-id="1b6d6-170">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1b6d6-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b6d6-171">Request</span></span>

<span data-ttu-id="1b6d6-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-172">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b6d6-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b6d6-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="1b6d6-174">C#</span><span class="sxs-lookup"><span data-stu-id="1b6d6-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b6d6-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b6d6-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b6d6-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b6d6-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b6d6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b6d6-177">Response</span></span>

<span data-ttu-id="1b6d6-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-178">The following is an example of the response.</span></span>

> <span data-ttu-id="1b6d6-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b6d6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
