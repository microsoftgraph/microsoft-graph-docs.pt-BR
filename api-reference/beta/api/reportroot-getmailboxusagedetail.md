---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2b3a6e40dcdb6def542ceff19f75c195c7f4a2c3
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983745"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="69e68-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="69e68-103">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="69e68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69e68-105">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="69e68-105">Get details about mailbox usage.</span></span>

> <span data-ttu-id="69e68-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="69e68-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="69e68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="69e68-107">Permissions</span></span>

<span data-ttu-id="69e68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69e68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69e68-110">Permission type</span></span>                        | <span data-ttu-id="69e68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69e68-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="69e68-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69e68-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="69e68-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69e68-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="69e68-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69e68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69e68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69e68-115">Not supported.</span></span>                           |
| <span data-ttu-id="69e68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69e68-116">Application</span></span>                            | <span data-ttu-id="69e68-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69e68-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="69e68-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="69e68-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="69e68-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="69e68-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="69e68-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69e68-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="69e68-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="69e68-121">Function parameters</span></span>

<span data-ttu-id="69e68-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="69e68-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="69e68-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="69e68-123">Parameter</span></span> | <span data-ttu-id="69e68-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="69e68-124">Type</span></span>   | <span data-ttu-id="69e68-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="69e68-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="69e68-126">ponto</span><span class="sxs-lookup"><span data-stu-id="69e68-126">period</span></span>    | <span data-ttu-id="69e68-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69e68-127">string</span></span> | <span data-ttu-id="69e68-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="69e68-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="69e68-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="69e68-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="69e68-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="69e68-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="69e68-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69e68-131">Required.</span></span> |

<span data-ttu-id="69e68-132">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="69e68-132">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="69e68-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="69e68-133">The default output type is text/csv.</span></span> <span data-ttu-id="69e68-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="69e68-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69e68-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69e68-135">Request headers</span></span>

| <span data-ttu-id="69e68-136">Nome</span><span class="sxs-lookup"><span data-stu-id="69e68-136">Name</span></span>          | <span data-ttu-id="69e68-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="69e68-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="69e68-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="69e68-138">Authorization</span></span> | <span data-ttu-id="69e68-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69e68-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="69e68-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="69e68-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="69e68-142">CSV</span><span class="sxs-lookup"><span data-stu-id="69e68-142">CSV</span></span>

<span data-ttu-id="69e68-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="69e68-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="69e68-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="69e68-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="69e68-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="69e68-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="69e68-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="69e68-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="69e68-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="69e68-147">Report Refresh Date</span></span>
- <span data-ttu-id="69e68-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="69e68-148">User Principal Name</span></span>
- <span data-ttu-id="69e68-149">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="69e68-149">Display Name</span></span>
- <span data-ttu-id="69e68-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="69e68-150">Is Deleted</span></span>
- <span data-ttu-id="69e68-151">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="69e68-151">Deleted Date</span></span>
- <span data-ttu-id="69e68-152">Data de criação</span><span class="sxs-lookup"><span data-stu-id="69e68-152">Created Date</span></span>
- <span data-ttu-id="69e68-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="69e68-153">Last Activity Date</span></span>
- <span data-ttu-id="69e68-154">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="69e68-154">Item Count</span></span>
- <span data-ttu-id="69e68-155">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="69e68-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="69e68-156">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="69e68-156">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="69e68-157">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="69e68-157">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="69e68-158">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="69e68-158">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="69e68-159">Contagem de itens excluídos</span><span class="sxs-lookup"><span data-stu-id="69e68-159">Deleted Item Count</span></span>
- <span data-ttu-id="69e68-160">Tamanho de itens excluídos (bytes)</span><span class="sxs-lookup"><span data-stu-id="69e68-160">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="69e68-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="69e68-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="69e68-162">JSON</span><span class="sxs-lookup"><span data-stu-id="69e68-162">JSON</span></span>

<span data-ttu-id="69e68-163">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69e68-163">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="69e68-164">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="69e68-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="69e68-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69e68-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="69e68-166">CSV</span><span class="sxs-lookup"><span data-stu-id="69e68-166">CSV</span></span>

<span data-ttu-id="69e68-167">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="69e68-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="69e68-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69e68-168">Request</span></span>

<span data-ttu-id="69e68-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69e68-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="69e68-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="69e68-170">Response</span></span>

<span data-ttu-id="69e68-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69e68-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="69e68-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="69e68-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="69e68-173">JSON</span><span class="sxs-lookup"><span data-stu-id="69e68-173">JSON</span></span>

<span data-ttu-id="69e68-174">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="69e68-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="69e68-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69e68-175">Request</span></span>

<span data-ttu-id="69e68-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69e68-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="69e68-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="69e68-177">Response</span></span>

<span data-ttu-id="69e68-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69e68-178">The following is an example of the response.</span></span>

> <span data-ttu-id="69e68-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69e68-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


