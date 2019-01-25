---
title: 'reportRoot: getEmailActivityCounts'
description: Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1482cf4ddef208c9cacb2d8efaa7eae0d43fda25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517152"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="189c6-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="189c6-103">reportRoot: getEmailActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="189c6-104">Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização.</span><span class="sxs-lookup"><span data-stu-id="189c6-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="189c6-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="189c6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="189c6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="189c6-106">Permissions</span></span>

<span data-ttu-id="189c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="189c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="189c6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="189c6-109">Permission type</span></span>                        | <span data-ttu-id="189c6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="189c6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="189c6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="189c6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="189c6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="189c6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="189c6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="189c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="189c6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="189c6-114">Not supported.</span></span>                           |
| <span data-ttu-id="189c6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="189c6-115">Application</span></span>                            | <span data-ttu-id="189c6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="189c6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="189c6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="189c6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="189c6-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="189c6-118">Function parameters</span></span>

<span data-ttu-id="189c6-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="189c6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="189c6-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="189c6-120">Parameter</span></span> | <span data-ttu-id="189c6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="189c6-121">Type</span></span>   | <span data-ttu-id="189c6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="189c6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="189c6-123">ponto</span><span class="sxs-lookup"><span data-stu-id="189c6-123">period</span></span>    | <span data-ttu-id="189c6-124">string</span><span class="sxs-lookup"><span data-stu-id="189c6-124">string</span></span> | <span data-ttu-id="189c6-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="189c6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="189c6-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="189c6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="189c6-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="189c6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="189c6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="189c6-128">Required.</span></span> |

<span data-ttu-id="189c6-129">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="189c6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="189c6-130">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="189c6-130">The default output type is text/csv.</span></span> <span data-ttu-id="189c6-131">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="189c6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="189c6-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="189c6-132">Request headers</span></span>

| <span data-ttu-id="189c6-133">Nome</span><span class="sxs-lookup"><span data-stu-id="189c6-133">Name</span></span>          | <span data-ttu-id="189c6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="189c6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="189c6-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="189c6-135">Authorization</span></span> | <span data-ttu-id="189c6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="189c6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="189c6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="189c6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="189c6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="189c6-139">CSV</span></span>

<span data-ttu-id="189c6-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="189c6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="189c6-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="189c6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="189c6-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="189c6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="189c6-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="189c6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="189c6-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="189c6-144">Report Refresh Date</span></span>
- <span data-ttu-id="189c6-145">Enviar</span><span class="sxs-lookup"><span data-stu-id="189c6-145">Send</span></span>
- <span data-ttu-id="189c6-146">Receber</span><span class="sxs-lookup"><span data-stu-id="189c6-146">Receive</span></span>
- <span data-ttu-id="189c6-147">Ler</span><span class="sxs-lookup"><span data-stu-id="189c6-147">Read</span></span>
- <span data-ttu-id="189c6-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="189c6-148">Report Date</span></span>
- <span data-ttu-id="189c6-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="189c6-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="189c6-150">JSON</span><span class="sxs-lookup"><span data-stu-id="189c6-150">JSON</span></span>

<span data-ttu-id="189c6-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailActivitySummary](../resources/emailactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="189c6-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="189c6-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="189c6-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="189c6-153">CSV</span><span class="sxs-lookup"><span data-stu-id="189c6-153">CSV</span></span>

<span data-ttu-id="189c6-154">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="189c6-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="189c6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="189c6-155">Request</span></span>

<span data-ttu-id="189c6-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="189c6-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="189c6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="189c6-157">Response</span></span>

<span data-ttu-id="189c6-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="189c6-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="189c6-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="189c6-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="189c6-160">JSON</span><span class="sxs-lookup"><span data-stu-id="189c6-160">JSON</span></span>

<span data-ttu-id="189c6-161">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="189c6-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="189c6-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="189c6-162">Request</span></span>

<span data-ttu-id="189c6-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="189c6-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="189c6-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="189c6-164">Response</span></span>

<span data-ttu-id="189c6-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="189c6-165">The following is an example of the response.</span></span>

> <span data-ttu-id="189c6-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="189c6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailactivitycounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
