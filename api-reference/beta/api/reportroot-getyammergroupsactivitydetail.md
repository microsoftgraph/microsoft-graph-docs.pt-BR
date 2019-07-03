---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Obtenha dados sobre as atividades de grupo do Yammer por grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 87329e35a8613162ee3d65da01d4a032701b7d84
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456166"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="0f336-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="0f336-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f336-104">Obtenha dados sobre as atividades de grupo do Yammer por grupo.</span><span class="sxs-lookup"><span data-stu-id="0f336-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="0f336-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="0f336-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f336-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f336-106">Permissions</span></span>

<span data-ttu-id="0f336-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f336-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f336-109">Permission type</span></span>                        | <span data-ttu-id="0f336-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f336-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0f336-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f336-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f336-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f336-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0f336-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f336-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f336-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f336-114">Not supported.</span></span>                           |
| <span data-ttu-id="0f336-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f336-115">Application</span></span>                            | <span data-ttu-id="0f336-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f336-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0f336-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f336-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0f336-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0f336-118">Function parameters</span></span>

<span data-ttu-id="0f336-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0f336-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0f336-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0f336-120">Parameter</span></span> | <span data-ttu-id="0f336-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f336-121">Type</span></span>   | <span data-ttu-id="0f336-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f336-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0f336-123">ponto</span><span class="sxs-lookup"><span data-stu-id="0f336-123">period</span></span>    | <span data-ttu-id="0f336-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f336-124">string</span></span> | <span data-ttu-id="0f336-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0f336-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0f336-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0f336-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0f336-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0f336-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0f336-128">data</span><span class="sxs-lookup"><span data-stu-id="0f336-128">date</span></span>      | <span data-ttu-id="0f336-129">Data</span><span class="sxs-lookup"><span data-stu-id="0f336-129">Date</span></span>   | <span data-ttu-id="0f336-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="0f336-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0f336-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0f336-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0f336-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="0f336-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0f336-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="0f336-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="0f336-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="0f336-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0f336-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="0f336-135">The default output type is text/csv.</span></span> <span data-ttu-id="0f336-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0f336-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f336-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f336-137">Request headers</span></span>

| <span data-ttu-id="0f336-138">Nome</span><span class="sxs-lookup"><span data-stu-id="0f336-138">Name</span></span>          | <span data-ttu-id="0f336-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f336-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0f336-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f336-140">Authorization</span></span> | <span data-ttu-id="0f336-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f336-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0f336-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f336-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0f336-144">CSV</span><span class="sxs-lookup"><span data-stu-id="0f336-144">CSV</span></span>

<span data-ttu-id="0f336-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0f336-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0f336-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0f336-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0f336-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0f336-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0f336-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0f336-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0f336-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0f336-149">Report Refresh Date</span></span>
- <span data-ttu-id="0f336-150">Nome de exibição do grupo</span><span class="sxs-lookup"><span data-stu-id="0f336-150">Group Display Name</span></span>
- <span data-ttu-id="0f336-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="0f336-151">Is Deleted</span></span>
- <span data-ttu-id="0f336-152">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="0f336-152">Owner Principal Name</span></span>
- <span data-ttu-id="0f336-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="0f336-153">Last Activity Date</span></span>
- <span data-ttu-id="0f336-154">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="0f336-154">Group Type</span></span>
- <span data-ttu-id="0f336-155">Office 365 Connected</span><span class="sxs-lookup"><span data-stu-id="0f336-155">Office 365 Connected</span></span>
- <span data-ttu-id="0f336-156">Contagem de Membros</span><span class="sxs-lookup"><span data-stu-id="0f336-156">Member Count</span></span>
- <span data-ttu-id="0f336-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="0f336-157">Posted Count</span></span>
- <span data-ttu-id="0f336-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="0f336-158">Read Count</span></span>
- <span data-ttu-id="0f336-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="0f336-159">Liked Count</span></span>
- <span data-ttu-id="0f336-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0f336-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0f336-161">JSON</span><span class="sxs-lookup"><span data-stu-id="0f336-161">JSON</span></span>

<span data-ttu-id="0f336-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f336-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="0f336-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="0f336-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="0f336-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f336-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0f336-165">CSV</span><span class="sxs-lookup"><span data-stu-id="0f336-165">CSV</span></span>

<span data-ttu-id="0f336-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="0f336-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0f336-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f336-167">Request</span></span>

<span data-ttu-id="0f336-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f336-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f336-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f336-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f336-170">C#</span><span class="sxs-lookup"><span data-stu-id="0f336-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f336-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="0f336-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f336-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f336-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f336-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f336-173">Response</span></span>

<span data-ttu-id="0f336-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f336-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0f336-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0f336-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="0f336-176">JSON</span><span class="sxs-lookup"><span data-stu-id="0f336-176">JSON</span></span>

<span data-ttu-id="0f336-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="0f336-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0f336-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f336-178">Request</span></span>

<span data-ttu-id="0f336-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f336-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f336-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f336-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f336-181">C#</span><span class="sxs-lookup"><span data-stu-id="0f336-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f336-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="0f336-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f336-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f336-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0f336-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f336-184">Response</span></span>

<span data-ttu-id="0f336-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f336-185">The following is an example of the response.</span></span>

> <span data-ttu-id="0f336-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f336-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
