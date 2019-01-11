---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório. Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.
localization_priority: Normal
ms.openlocfilehash: c1b15824ab5313d1c581509936a84f5af2daee84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856284"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="4a4bf-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="4a4bf-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

> <span data-ttu-id="4a4bf-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a4bf-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a4bf-107">Obtenha o número total de caixas de correio de usuários em sua organização e quantas são ativas a cada dia do período de relatório.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-107">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="4a4bf-108">Uma caixa postal é considerada ativa se o usuário enviou ou leu qualquer email.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-108">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="4a4bf-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="4a4bf-109">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a4bf-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a4bf-110">Permissions</span></span>

<span data-ttu-id="4a4bf-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a4bf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a4bf-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a4bf-113">Permission type</span></span>                        | <span data-ttu-id="4a4bf-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a4bf-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4a4bf-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a4bf-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a4bf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a4bf-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4a4bf-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a4bf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a4bf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-118">Not supported.</span></span>                           |
| <span data-ttu-id="4a4bf-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a4bf-119">Application</span></span>                            | <span data-ttu-id="4a4bf-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a4bf-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4a4bf-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a4bf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4a4bf-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4a4bf-122">Function parameters</span></span>

<span data-ttu-id="4a4bf-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4a4bf-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4a4bf-124">Parameter</span></span> | <span data-ttu-id="4a4bf-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a4bf-125">Type</span></span>   | <span data-ttu-id="4a4bf-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a4bf-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4a4bf-127">ponto</span><span class="sxs-lookup"><span data-stu-id="4a4bf-127">period</span></span>    | <span data-ttu-id="4a4bf-128">string</span><span class="sxs-lookup"><span data-stu-id="4a4bf-128">string</span></span> | <span data-ttu-id="4a4bf-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4a4bf-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4a4bf-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4a4bf-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-132">Required.</span></span> |

<span data-ttu-id="4a4bf-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4a4bf-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-134">The default output type is text/csv.</span></span> <span data-ttu-id="4a4bf-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a4bf-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4bf-136">Request headers</span></span>

| <span data-ttu-id="4a4bf-137">Nome</span><span class="sxs-lookup"><span data-stu-id="4a4bf-137">Name</span></span>          | <span data-ttu-id="4a4bf-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a4bf-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4a4bf-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a4bf-139">Authorization</span></span> | <span data-ttu-id="4a4bf-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4a4bf-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a4bf-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4a4bf-143">CSV</span><span class="sxs-lookup"><span data-stu-id="4a4bf-143">CSV</span></span>

<span data-ttu-id="4a4bf-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4a4bf-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4a4bf-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4a4bf-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4a4bf-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4a4bf-148">Report Refresh Date</span></span>
- <span data-ttu-id="4a4bf-149">Total</span><span class="sxs-lookup"><span data-stu-id="4a4bf-149">Total</span></span>
- <span data-ttu-id="4a4bf-150">Ativo</span><span class="sxs-lookup"><span data-stu-id="4a4bf-150">Active</span></span>
- <span data-ttu-id="4a4bf-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4a4bf-151">Report Date</span></span>
- <span data-ttu-id="4a4bf-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4a4bf-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4a4bf-153">JSON</span><span class="sxs-lookup"><span data-stu-id="4a4bf-153">JSON</span></span>

<span data-ttu-id="4a4bf-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-154">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a4bf-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a4bf-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4a4bf-156">CSV</span><span class="sxs-lookup"><span data-stu-id="4a4bf-156">CSV</span></span>

<span data-ttu-id="4a4bf-157">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4a4bf-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4bf-158">Request</span></span>

<span data-ttu-id="4a4bf-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4a4bf-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a4bf-160">Response</span></span>

<span data-ttu-id="4a4bf-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4a4bf-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4a4bf-163">JSON</span><span class="sxs-lookup"><span data-stu-id="4a4bf-163">JSON</span></span>

<span data-ttu-id="4a4bf-164">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4a4bf-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4bf-165">Request</span></span>

<span data-ttu-id="4a4bf-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4a4bf-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a4bf-167">Response</span></span>

<span data-ttu-id="4a4bf-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-168">The following is an example of the response.</span></span>

> <span data-ttu-id="4a4bf-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a4bf-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
