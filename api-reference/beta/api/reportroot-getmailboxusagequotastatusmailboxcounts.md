---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: c58c3a0202f099cd10eab01c152c17cba5f00719
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981645"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="8d8aa-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="8d8aa-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

<span data-ttu-id="8d8aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d8aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d8aa-105">Obtenha a contagem de caixas de correio de usuário em cada categoria de cota.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-105">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="8d8aa-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="8d8aa-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d8aa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d8aa-107">Permissions</span></span>

<span data-ttu-id="8d8aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d8aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d8aa-110">Permission type</span></span>                        | <span data-ttu-id="8d8aa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d8aa-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8d8aa-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d8aa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d8aa-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d8aa-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8d8aa-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d8aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d8aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-115">Not supported.</span></span>                           |
| <span data-ttu-id="8d8aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d8aa-116">Application</span></span>                            | <span data-ttu-id="8d8aa-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d8aa-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="8d8aa-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="8d8aa-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="8d8aa-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="8d8aa-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d8aa-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8d8aa-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8d8aa-121">Function parameters</span></span>

<span data-ttu-id="8d8aa-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8d8aa-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d8aa-123">Parameter</span></span> | <span data-ttu-id="8d8aa-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d8aa-124">Type</span></span>   | <span data-ttu-id="8d8aa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d8aa-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8d8aa-126">ponto</span><span class="sxs-lookup"><span data-stu-id="8d8aa-126">period</span></span>    | <span data-ttu-id="8d8aa-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d8aa-127">string</span></span> | <span data-ttu-id="8d8aa-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8d8aa-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8d8aa-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8d8aa-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-131">Required.</span></span> |

<span data-ttu-id="8d8aa-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8d8aa-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-133">The default output type is text/csv.</span></span> <span data-ttu-id="8d8aa-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d8aa-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8aa-135">Request headers</span></span>

| <span data-ttu-id="8d8aa-136">Nome</span><span class="sxs-lookup"><span data-stu-id="8d8aa-136">Name</span></span>          | <span data-ttu-id="8d8aa-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d8aa-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8d8aa-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d8aa-138">Authorization</span></span> | <span data-ttu-id="8d8aa-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8d8aa-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d8aa-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8d8aa-142">CSV</span><span class="sxs-lookup"><span data-stu-id="8d8aa-142">CSV</span></span>

<span data-ttu-id="8d8aa-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8d8aa-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8d8aa-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8d8aa-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8d8aa-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8d8aa-147">Report Refresh Date</span></span>
- <span data-ttu-id="8d8aa-148">Abaixo do limite</span><span class="sxs-lookup"><span data-stu-id="8d8aa-148">Under Limit</span></span>
- <span data-ttu-id="8d8aa-149">Aviso emitido</span><span class="sxs-lookup"><span data-stu-id="8d8aa-149">Warning Issued</span></span>
- <span data-ttu-id="8d8aa-150">Envio proibido</span><span class="sxs-lookup"><span data-stu-id="8d8aa-150">Send Prohibited</span></span>
- <span data-ttu-id="8d8aa-151">Envio/recebimento proibido</span><span class="sxs-lookup"><span data-stu-id="8d8aa-151">Send/Receive Prohibited</span></span>
- <span data-ttu-id="8d8aa-152">Indeterminado</span><span class="sxs-lookup"><span data-stu-id="8d8aa-152">Indeterminate</span></span>
- <span data-ttu-id="8d8aa-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="8d8aa-153">Report Date</span></span>
- <span data-ttu-id="8d8aa-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8d8aa-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8d8aa-155">JSON</span><span class="sxs-lookup"><span data-stu-id="8d8aa-155">JSON</span></span>

<span data-ttu-id="8d8aa-156">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-156">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d8aa-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d8aa-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8d8aa-158">CSV</span><span class="sxs-lookup"><span data-stu-id="8d8aa-158">CSV</span></span>

<span data-ttu-id="8d8aa-159">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8d8aa-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8aa-160">Request</span></span>

<span data-ttu-id="8d8aa-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="8d8aa-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d8aa-162">Response</span></span>

<span data-ttu-id="8d8aa-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8d8aa-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8d8aa-165">JSON</span><span class="sxs-lookup"><span data-stu-id="8d8aa-165">JSON</span></span>

<span data-ttu-id="8d8aa-166">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8d8aa-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d8aa-167">Request</span></span>

<span data-ttu-id="8d8aa-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="8d8aa-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d8aa-169">Response</span></span>

<span data-ttu-id="8d8aa-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-170">The following is an example of the response.</span></span>

> <span data-ttu-id="8d8aa-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d8aa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


