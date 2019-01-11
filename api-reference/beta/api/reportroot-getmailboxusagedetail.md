---
title: 'reportRoot: getMailboxUsageDetail'
description: Obtenha dados sobre o uso da caixa de correio.
localization_priority: Normal
ms.openlocfilehash: 09fbb0ce1a4c652d4e24194b36edd790b1ec63f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865153"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="91b62-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="91b62-103">reportRoot: getMailboxUsageDetail</span></span>

> <span data-ttu-id="91b62-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91b62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91b62-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91b62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91b62-106">Obtenha dados sobre o uso da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="91b62-106">Get details about mailbox usage.</span></span>

> <span data-ttu-id="91b62-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="91b62-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="91b62-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="91b62-108">Permissions</span></span>

<span data-ttu-id="91b62-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91b62-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91b62-111">Permission type</span></span>                        | <span data-ttu-id="91b62-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91b62-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="91b62-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91b62-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="91b62-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b62-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="91b62-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91b62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91b62-116">Not supported.</span></span>                           |
| <span data-ttu-id="91b62-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91b62-117">Application</span></span>                            | <span data-ttu-id="91b62-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b62-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="91b62-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91b62-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="91b62-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="91b62-120">Function parameters</span></span>

<span data-ttu-id="91b62-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="91b62-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="91b62-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="91b62-122">Parameter</span></span> | <span data-ttu-id="91b62-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b62-123">Type</span></span>   | <span data-ttu-id="91b62-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b62-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="91b62-125">ponto</span><span class="sxs-lookup"><span data-stu-id="91b62-125">period</span></span>    | <span data-ttu-id="91b62-126">string</span><span class="sxs-lookup"><span data-stu-id="91b62-126">string</span></span> | <span data-ttu-id="91b62-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="91b62-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="91b62-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="91b62-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="91b62-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="91b62-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="91b62-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b62-130">Required.</span></span> |

<span data-ttu-id="91b62-131">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="91b62-131">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="91b62-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="91b62-132">The default output type is text/csv.</span></span> <span data-ttu-id="91b62-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="91b62-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91b62-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91b62-134">Request headers</span></span>

| <span data-ttu-id="91b62-135">Nome</span><span class="sxs-lookup"><span data-stu-id="91b62-135">Name</span></span>          | <span data-ttu-id="91b62-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b62-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="91b62-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="91b62-137">Authorization</span></span> | <span data-ttu-id="91b62-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b62-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="91b62-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b62-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="91b62-141">CSV</span><span class="sxs-lookup"><span data-stu-id="91b62-141">CSV</span></span>

<span data-ttu-id="91b62-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="91b62-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="91b62-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="91b62-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="91b62-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="91b62-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="91b62-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="91b62-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="91b62-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="91b62-146">Report Refresh Date</span></span>
- <span data-ttu-id="91b62-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="91b62-147">User Principal Name</span></span>
- <span data-ttu-id="91b62-148">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="91b62-148">Display Name</span></span>
- <span data-ttu-id="91b62-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="91b62-149">Is Deleted</span></span>
- <span data-ttu-id="91b62-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="91b62-150">Deleted Date</span></span>
- <span data-ttu-id="91b62-151">Data de criação</span><span class="sxs-lookup"><span data-stu-id="91b62-151">Created Date</span></span>
- <span data-ttu-id="91b62-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="91b62-152">Last Activity Date</span></span>
- <span data-ttu-id="91b62-153">Contagem de itens</span><span class="sxs-lookup"><span data-stu-id="91b62-153">Item Count</span></span>
- <span data-ttu-id="91b62-154">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="91b62-154">Storage Used (Byte)</span></span>
- <span data-ttu-id="91b62-155">Cota de aviso de problema (bytes)</span><span class="sxs-lookup"><span data-stu-id="91b62-155">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="91b62-156">Cota de proibição de envio (bytes)</span><span class="sxs-lookup"><span data-stu-id="91b62-156">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="91b62-157">Cota de envio/recebimento (bytes)</span><span class="sxs-lookup"><span data-stu-id="91b62-157">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="91b62-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="91b62-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="91b62-159">JSON</span><span class="sxs-lookup"><span data-stu-id="91b62-159">JSON</span></span>

<span data-ttu-id="91b62-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b62-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="91b62-161">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="91b62-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="91b62-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91b62-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="91b62-163">CSV</span><span class="sxs-lookup"><span data-stu-id="91b62-163">CSV</span></span>

<span data-ttu-id="91b62-164">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="91b62-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="91b62-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91b62-165">Request</span></span>

<span data-ttu-id="91b62-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b62-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="91b62-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b62-167">Response</span></span>

<span data-ttu-id="91b62-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91b62-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="91b62-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="91b62-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="91b62-170">JSON</span><span class="sxs-lookup"><span data-stu-id="91b62-170">JSON</span></span>

<span data-ttu-id="91b62-171">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="91b62-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="91b62-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91b62-172">Request</span></span>

<span data-ttu-id="91b62-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b62-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="91b62-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b62-174">Response</span></span>

<span data-ttu-id="91b62-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91b62-175">The following is an example of the response.</span></span>

> <span data-ttu-id="91b62-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91b62-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
