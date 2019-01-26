---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2b9f9b9661236e20964245f8e89d17c013f40800
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571223"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="01b26-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="01b26-103">reportRoot: getEmailActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01b26-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="01b26-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="01b26-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="01b26-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="01b26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="01b26-106">Permissions</span></span>

<span data-ttu-id="01b26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01b26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01b26-109">Permission type</span></span>                        | <span data-ttu-id="01b26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01b26-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="01b26-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01b26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01b26-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b26-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="01b26-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01b26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01b26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01b26-114">Not supported.</span></span>                           |
| <span data-ttu-id="01b26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01b26-115">Application</span></span>                            | <span data-ttu-id="01b26-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b26-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="01b26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01b26-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="01b26-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="01b26-118">Function parameters</span></span>

<span data-ttu-id="01b26-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="01b26-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="01b26-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01b26-120">Parameter</span></span> | <span data-ttu-id="01b26-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="01b26-121">Type</span></span>   | <span data-ttu-id="01b26-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="01b26-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="01b26-123">ponto</span><span class="sxs-lookup"><span data-stu-id="01b26-123">period</span></span>    | <span data-ttu-id="01b26-124">string</span><span class="sxs-lookup"><span data-stu-id="01b26-124">string</span></span> | <span data-ttu-id="01b26-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01b26-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="01b26-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="01b26-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="01b26-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01b26-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="01b26-128">data</span><span class="sxs-lookup"><span data-stu-id="01b26-128">date</span></span>      | <span data-ttu-id="01b26-129">Data</span><span class="sxs-lookup"><span data-stu-id="01b26-129">Date</span></span>   | <span data-ttu-id="01b26-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="01b26-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="01b26-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="01b26-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="01b26-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="01b26-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="01b26-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="01b26-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="01b26-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="01b26-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="01b26-135">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="01b26-135">The default output type is text/csv.</span></span> <span data-ttu-id="01b26-136">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="01b26-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01b26-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01b26-137">Request headers</span></span>

| <span data-ttu-id="01b26-138">Nome</span><span class="sxs-lookup"><span data-stu-id="01b26-138">Name</span></span>          | <span data-ttu-id="01b26-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="01b26-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="01b26-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="01b26-140">Authorization</span></span> | <span data-ttu-id="01b26-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01b26-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="01b26-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b26-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="01b26-144">CSV</span><span class="sxs-lookup"><span data-stu-id="01b26-144">CSV</span></span>

<span data-ttu-id="01b26-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="01b26-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="01b26-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="01b26-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="01b26-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="01b26-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="01b26-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="01b26-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="01b26-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="01b26-149">Report Refresh Date</span></span>
- <span data-ttu-id="01b26-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="01b26-150">User Principal Name</span></span>
- <span data-ttu-id="01b26-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="01b26-151">Display Name</span></span>
- <span data-ttu-id="01b26-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="01b26-152">Is Deleted</span></span>
- <span data-ttu-id="01b26-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="01b26-153">Deleted Date</span></span>
- <span data-ttu-id="01b26-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="01b26-154">Last Activity Date</span></span>
- <span data-ttu-id="01b26-155">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="01b26-155">Send Count</span></span>
- <span data-ttu-id="01b26-156">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="01b26-156">Receive Count</span></span>
- <span data-ttu-id="01b26-157">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="01b26-157">Read Count</span></span>
- <span data-ttu-id="01b26-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="01b26-158">Assigned Products</span></span>
- <span data-ttu-id="01b26-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="01b26-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="01b26-160">JSON</span><span class="sxs-lookup"><span data-stu-id="01b26-160">JSON</span></span>

<span data-ttu-id="01b26-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01b26-161">If successful, this method returns a `200 OK` response code and an **[emailActivityUserDetail](../resources/emailactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="01b26-162">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="01b26-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="01b26-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01b26-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="01b26-164">CSV</span><span class="sxs-lookup"><span data-stu-id="01b26-164">CSV</span></span>

<span data-ttu-id="01b26-165">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="01b26-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="01b26-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01b26-166">Request</span></span>

<span data-ttu-id="01b26-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01b26-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="01b26-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b26-168">Response</span></span>

<span data-ttu-id="01b26-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01b26-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="01b26-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="01b26-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="01b26-171">JSON</span><span class="sxs-lookup"><span data-stu-id="01b26-171">JSON</span></span>

<span data-ttu-id="01b26-172">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="01b26-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="01b26-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01b26-173">Request</span></span>

<span data-ttu-id="01b26-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01b26-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="01b26-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="01b26-175">Response</span></span>

<span data-ttu-id="01b26-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01b26-176">The following is an example of the response.</span></span>

> <span data-ttu-id="01b26-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01b26-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
