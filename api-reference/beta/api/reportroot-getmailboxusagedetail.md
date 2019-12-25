---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 51b3a99c3ee9e010e41171dccf8f3d07329bf954
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869182"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="d81b6-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="d81b6-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d81b6-104">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d81b6-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="d81b6-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="d81b6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="d81b6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d81b6-106">Permissions</span></span>

<span data-ttu-id="d81b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d81b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d81b6-109">Permission type</span></span>                        | <span data-ttu-id="d81b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d81b6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d81b6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d81b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d81b6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d81b6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d81b6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d81b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d81b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d81b6-114">Not supported.</span></span>                           |
| <span data-ttu-id="d81b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d81b6-115">Application</span></span>                            | <span data-ttu-id="d81b6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d81b6-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="d81b6-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="d81b6-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d81b6-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d81b6-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d81b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d81b6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d81b6-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d81b6-120">Function parameters</span></span>

<span data-ttu-id="d81b6-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d81b6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d81b6-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d81b6-122">Parameter</span></span> | <span data-ttu-id="d81b6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d81b6-123">Type</span></span>   | <span data-ttu-id="d81b6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81b6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d81b6-125">ponto</span><span class="sxs-lookup"><span data-stu-id="d81b6-125">period</span></span>    | <span data-ttu-id="d81b6-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d81b6-126">string</span></span> | <span data-ttu-id="d81b6-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d81b6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d81b6-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d81b6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d81b6-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d81b6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d81b6-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81b6-130">Required.</span></span> |

<span data-ttu-id="d81b6-131">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="d81b6-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d81b6-132">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d81b6-132">The default output type is text/csv.</span></span> <span data-ttu-id="d81b6-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d81b6-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d81b6-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d81b6-134">Request headers</span></span>

| <span data-ttu-id="d81b6-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d81b6-135">Name</span></span>          | <span data-ttu-id="d81b6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d81b6-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d81b6-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d81b6-137">Authorization</span></span> | <span data-ttu-id="d81b6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d81b6-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d81b6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81b6-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d81b6-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d81b6-141">CSV</span></span>

<span data-ttu-id="d81b6-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d81b6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d81b6-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d81b6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d81b6-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d81b6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d81b6-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d81b6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d81b6-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d81b6-146">Report Refresh Date</span></span>
- <span data-ttu-id="d81b6-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="d81b6-147">User Principal Name</span></span>
- <span data-ttu-id="d81b6-148">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="d81b6-148">Display Name</span></span>
- <span data-ttu-id="d81b6-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="d81b6-149">Is Deleted</span></span>
- <span data-ttu-id="d81b6-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="d81b6-150">Deleted Date</span></span>
- <span data-ttu-id="d81b6-151">Data de criação</span><span class="sxs-lookup"><span data-stu-id="d81b6-151">Created Date</span></span>
- <span data-ttu-id="d81b6-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="d81b6-152">Last Activity Date</span></span>
- <span data-ttu-id="d81b6-153">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="d81b6-153">Item Count</span></span>
- <span data-ttu-id="d81b6-154">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="d81b6-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="d81b6-155">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="d81b6-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="d81b6-156">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="d81b6-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="d81b6-157">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="d81b6-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="d81b6-158">Contagem de itens excluídos</span><span class="sxs-lookup"><span data-stu-id="d81b6-158">Deleted Item Count</span></span>
- <span data-ttu-id="d81b6-159">Tamanho de itens excluídos (bytes)</span><span class="sxs-lookup"><span data-stu-id="d81b6-159">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="d81b6-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d81b6-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d81b6-161">JSON</span><span class="sxs-lookup"><span data-stu-id="d81b6-161">JSON</span></span>

<span data-ttu-id="d81b6-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d81b6-162">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="d81b6-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="d81b6-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d81b6-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d81b6-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d81b6-165">CSV</span><span class="sxs-lookup"><span data-stu-id="d81b6-165">CSV</span></span>

<span data-ttu-id="d81b6-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d81b6-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d81b6-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81b6-167">Request</span></span>

<span data-ttu-id="d81b6-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81b6-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d81b6-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81b6-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d81b6-170">C#</span><span class="sxs-lookup"><span data-stu-id="d81b6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d81b6-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81b6-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d81b6-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81b6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d81b6-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81b6-173">Response</span></span>

<span data-ttu-id="d81b6-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d81b6-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d81b6-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d81b6-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="d81b6-176">JSON</span><span class="sxs-lookup"><span data-stu-id="d81b6-176">JSON</span></span>

<span data-ttu-id="d81b6-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d81b6-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d81b6-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d81b6-178">Request</span></span>

<span data-ttu-id="d81b6-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d81b6-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d81b6-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81b6-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d81b6-181">C#</span><span class="sxs-lookup"><span data-stu-id="d81b6-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d81b6-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81b6-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d81b6-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81b6-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d81b6-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="d81b6-184">Response</span></span>

<span data-ttu-id="d81b6-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d81b6-185">The following is an example of the response.</span></span>

> <span data-ttu-id="d81b6-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d81b6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "deletedItemCount": 138481,
      "deletedItemSizeInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
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
