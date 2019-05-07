---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e6a695fd3d4bfdde1f64b4fee6d438420aa0191f
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639464"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="a2e05-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a2e05-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e05-104">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a2e05-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="a2e05-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a2e05-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a2e05-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2e05-106">Permissions</span></span>

<span data-ttu-id="a2e05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2e05-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2e05-109">Permission type</span></span>                        | <span data-ttu-id="a2e05-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2e05-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a2e05-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2e05-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2e05-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2e05-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a2e05-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2e05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2e05-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2e05-114">Not supported.</span></span>                           |
| <span data-ttu-id="a2e05-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2e05-115">Application</span></span>                            | <span data-ttu-id="a2e05-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2e05-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a2e05-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2e05-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a2e05-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a2e05-118">Function parameters</span></span>

<span data-ttu-id="a2e05-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a2e05-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a2e05-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a2e05-120">Parameter</span></span> | <span data-ttu-id="a2e05-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2e05-121">Type</span></span>   | <span data-ttu-id="a2e05-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e05-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a2e05-123">ponto</span><span class="sxs-lookup"><span data-stu-id="a2e05-123">period</span></span>    | <span data-ttu-id="a2e05-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2e05-124">string</span></span> | <span data-ttu-id="a2e05-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a2e05-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a2e05-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a2e05-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a2e05-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a2e05-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a2e05-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e05-128">Required.</span></span> |

<span data-ttu-id="a2e05-129">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e05-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a2e05-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="a2e05-130">The default output type is text/csv.</span></span> <span data-ttu-id="a2e05-131">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a2e05-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2e05-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e05-132">Request headers</span></span>

| <span data-ttu-id="a2e05-133">Nome</span><span class="sxs-lookup"><span data-stu-id="a2e05-133">Name</span></span>          | <span data-ttu-id="a2e05-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e05-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2e05-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2e05-135">Authorization</span></span> | <span data-ttu-id="a2e05-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e05-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a2e05-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e05-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a2e05-139">CSV</span><span class="sxs-lookup"><span data-stu-id="a2e05-139">CSV</span></span>

<span data-ttu-id="a2e05-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a2e05-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a2e05-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e05-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a2e05-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a2e05-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a2e05-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a2e05-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a2e05-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a2e05-144">Report Refresh Date</span></span>
- <span data-ttu-id="a2e05-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a2e05-145">User Principal Name</span></span>
- <span data-ttu-id="a2e05-146">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a2e05-146">Display Name</span></span>
- <span data-ttu-id="a2e05-147">Excluído</span><span class="sxs-lookup"><span data-stu-id="a2e05-147">Is Deleted</span></span>
- <span data-ttu-id="a2e05-148">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="a2e05-148">Deleted Date</span></span>
- <span data-ttu-id="a2e05-149">Data de criação</span><span class="sxs-lookup"><span data-stu-id="a2e05-149">Created Date</span></span>
- <span data-ttu-id="a2e05-150">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="a2e05-150">Last Activity Date</span></span>
- <span data-ttu-id="a2e05-151">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="a2e05-151">Item Count</span></span>
- <span data-ttu-id="a2e05-152">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a2e05-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="a2e05-153">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="a2e05-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="a2e05-154">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="a2e05-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="a2e05-155">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="a2e05-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="a2e05-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a2e05-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a2e05-157">JSON</span><span class="sxs-lookup"><span data-stu-id="a2e05-157">JSON</span></span>

<span data-ttu-id="a2e05-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e05-158">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="a2e05-159">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="a2e05-159">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a2e05-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2e05-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a2e05-161">CSV</span><span class="sxs-lookup"><span data-stu-id="a2e05-161">CSV</span></span>

<span data-ttu-id="a2e05-162">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="a2e05-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a2e05-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e05-163">Request</span></span>

<span data-ttu-id="a2e05-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2e05-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a2e05-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e05-165">Response</span></span>

<span data-ttu-id="a2e05-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e05-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2e05-167">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a2e05-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2e05-168">Basic</span><span class="sxs-lookup"><span data-stu-id="a2e05-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagedetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2e05-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2e05-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagedetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="a2e05-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a2e05-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="a2e05-171">JSON</span><span class="sxs-lookup"><span data-stu-id="a2e05-171">JSON</span></span>

<span data-ttu-id="a2e05-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="a2e05-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a2e05-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e05-173">Request</span></span>

<span data-ttu-id="a2e05-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2e05-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a2e05-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e05-175">Response</span></span>

<span data-ttu-id="a2e05-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e05-176">The following is an example of the response.</span></span>

> <span data-ttu-id="a2e05-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2e05-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2e05-179">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a2e05-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2e05-180">Basic</span><span class="sxs-lookup"><span data-stu-id="a2e05-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagedetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2e05-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2e05-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagedetail_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagedetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
