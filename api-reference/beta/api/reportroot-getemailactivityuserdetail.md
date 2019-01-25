---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: cfd4990c9e4f220f37146fc21747087b8d06f4e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521240"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="2a183-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2a183-103">reportRoot: getEmailActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a183-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="2a183-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="2a183-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="2a183-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a183-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a183-106">Permissions</span></span>

<span data-ttu-id="2a183-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a183-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a183-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a183-109">Permission type</span></span>                        | <span data-ttu-id="2a183-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a183-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2a183-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a183-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a183-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a183-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2a183-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a183-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a183-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a183-114">Not supported.</span></span>                           |
| <span data-ttu-id="2a183-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a183-115">Application</span></span>                            | <span data-ttu-id="2a183-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a183-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2a183-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a183-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2a183-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2a183-118">Function parameters</span></span>

<span data-ttu-id="2a183-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2a183-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2a183-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2a183-120">Parameter</span></span> | <span data-ttu-id="2a183-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a183-121">Type</span></span>   | <span data-ttu-id="2a183-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a183-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2a183-123">ponto</span><span class="sxs-lookup"><span data-stu-id="2a183-123">period</span></span>    | <span data-ttu-id="2a183-124">string</span><span class="sxs-lookup"><span data-stu-id="2a183-124">string</span></span> | <span data-ttu-id="2a183-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2a183-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2a183-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2a183-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2a183-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2a183-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2a183-128">data</span><span class="sxs-lookup"><span data-stu-id="2a183-128">date</span></span>      | <span data-ttu-id="2a183-129">Data</span><span class="sxs-lookup"><span data-stu-id="2a183-129">Date</span></span>   | <span data-ttu-id="2a183-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="2a183-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2a183-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="2a183-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2a183-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="2a183-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2a183-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="2a183-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="2a183-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="2a183-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2a183-135">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="2a183-135">The default output type is text/csv.</span></span> <span data-ttu-id="2a183-136">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="2a183-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a183-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a183-137">Request headers</span></span>

| <span data-ttu-id="2a183-138">Nome</span><span class="sxs-lookup"><span data-stu-id="2a183-138">Name</span></span>          | <span data-ttu-id="2a183-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a183-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2a183-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a183-140">Authorization</span></span> | <span data-ttu-id="2a183-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a183-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2a183-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a183-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2a183-144">CSV</span><span class="sxs-lookup"><span data-stu-id="2a183-144">CSV</span></span>

<span data-ttu-id="2a183-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2a183-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2a183-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2a183-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2a183-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2a183-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2a183-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2a183-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2a183-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2a183-149">Report Refresh Date</span></span>
- <span data-ttu-id="2a183-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="2a183-150">User Principal Name</span></span>
- <span data-ttu-id="2a183-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="2a183-151">Display Name</span></span>
- <span data-ttu-id="2a183-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="2a183-152">Is Deleted</span></span>
- <span data-ttu-id="2a183-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="2a183-153">Deleted Date</span></span>
- <span data-ttu-id="2a183-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="2a183-154">Last Activity Date</span></span>
- <span data-ttu-id="2a183-155">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="2a183-155">Send Count</span></span>
- <span data-ttu-id="2a183-156">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="2a183-156">Receive Count</span></span>
- <span data-ttu-id="2a183-157">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="2a183-157">Read Count</span></span>
- <span data-ttu-id="2a183-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="2a183-158">Assigned Products</span></span>
- <span data-ttu-id="2a183-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2a183-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2a183-160">JSON</span><span class="sxs-lookup"><span data-stu-id="2a183-160">JSON</span></span>

<span data-ttu-id="2a183-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a183-161">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="2a183-162">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="2a183-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="2a183-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a183-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2a183-164">CSV</span><span class="sxs-lookup"><span data-stu-id="2a183-164">CSV</span></span>

<span data-ttu-id="2a183-165">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="2a183-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2a183-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a183-166">Request</span></span>

<span data-ttu-id="2a183-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a183-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2a183-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a183-168">Response</span></span>

<span data-ttu-id="2a183-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a183-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2a183-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2a183-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="2a183-171">JSON</span><span class="sxs-lookup"><span data-stu-id="2a183-171">JSON</span></span>

<span data-ttu-id="2a183-172">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="2a183-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2a183-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a183-173">Request</span></span>

<span data-ttu-id="2a183-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a183-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2a183-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a183-175">Response</span></span>

<span data-ttu-id="2a183-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a183-176">The following is an example of the response.</span></span>

> <span data-ttu-id="2a183-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a183-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "sendCount": 86, 
      "receiveCount": 3198, 
      "readCount": 388, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getemailactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
