---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cf6ea4a5f696a302d9296f0719b1b322d5b0434b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446343"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="1bd17-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1bd17-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bd17-104">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="1bd17-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="1bd17-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="1bd17-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bd17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bd17-106">Permissions</span></span>

<span data-ttu-id="1bd17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bd17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bd17-109">Permission type</span></span>                        | <span data-ttu-id="1bd17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bd17-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1bd17-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bd17-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bd17-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bd17-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1bd17-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bd17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bd17-114">Not supported.</span></span>                           |
| <span data-ttu-id="1bd17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bd17-115">Application</span></span>                            | <span data-ttu-id="1bd17-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bd17-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1bd17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd17-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1bd17-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1bd17-118">Function parameters</span></span>

<span data-ttu-id="1bd17-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1bd17-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1bd17-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1bd17-120">Parameter</span></span> | <span data-ttu-id="1bd17-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd17-121">Type</span></span>   | <span data-ttu-id="1bd17-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd17-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1bd17-123">ponto</span><span class="sxs-lookup"><span data-stu-id="1bd17-123">period</span></span>    | <span data-ttu-id="1bd17-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd17-124">string</span></span> | <span data-ttu-id="1bd17-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1bd17-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1bd17-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1bd17-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1bd17-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1bd17-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1bd17-128">data</span><span class="sxs-lookup"><span data-stu-id="1bd17-128">date</span></span>      | <span data-ttu-id="1bd17-129">Data</span><span class="sxs-lookup"><span data-stu-id="1bd17-129">Date</span></span>   | <span data-ttu-id="1bd17-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="1bd17-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1bd17-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="1bd17-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1bd17-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="1bd17-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1bd17-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="1bd17-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="1bd17-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd17-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1bd17-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1bd17-135">The default output type is text/csv.</span></span> <span data-ttu-id="1bd17-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd17-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bd17-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd17-137">Request headers</span></span>

| <span data-ttu-id="1bd17-138">Nome</span><span class="sxs-lookup"><span data-stu-id="1bd17-138">Name</span></span>          | <span data-ttu-id="1bd17-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd17-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1bd17-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bd17-140">Authorization</span></span> | <span data-ttu-id="1bd17-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd17-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1bd17-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd17-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1bd17-144">CSV</span><span class="sxs-lookup"><span data-stu-id="1bd17-144">CSV</span></span>

<span data-ttu-id="1bd17-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1bd17-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1bd17-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd17-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1bd17-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1bd17-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1bd17-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1bd17-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1bd17-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1bd17-149">Report Refresh Date</span></span>
- <span data-ttu-id="1bd17-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="1bd17-150">User Principal Name</span></span>
- <span data-ttu-id="1bd17-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="1bd17-151">Display Name</span></span>
- <span data-ttu-id="1bd17-152">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="1bd17-152">User State</span></span>
- <span data-ttu-id="1bd17-153">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="1bd17-153">State Change Date</span></span>
- <span data-ttu-id="1bd17-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="1bd17-154">Last Activity Date</span></span>
- <span data-ttu-id="1bd17-155">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="1bd17-155">Posted Count</span></span>
- <span data-ttu-id="1bd17-156">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="1bd17-156">Read Count</span></span>
- <span data-ttu-id="1bd17-157">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="1bd17-157">Liked Count</span></span>
- <span data-ttu-id="1bd17-158">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="1bd17-158">Assigned Products</span></span>
- <span data-ttu-id="1bd17-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1bd17-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1bd17-160">JSON</span><span class="sxs-lookup"><span data-stu-id="1bd17-160">JSON</span></span>

<span data-ttu-id="1bd17-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd17-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="1bd17-162">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="1bd17-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="1bd17-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bd17-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1bd17-164">CSV</span><span class="sxs-lookup"><span data-stu-id="1bd17-164">CSV</span></span>

<span data-ttu-id="1bd17-165">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1bd17-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1bd17-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd17-166">Request</span></span>

<span data-ttu-id="1bd17-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bd17-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1bd17-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd17-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bd17-169">C#</span><span class="sxs-lookup"><span data-stu-id="1bd17-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bd17-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bd17-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bd17-171">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bd17-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1bd17-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd17-172">Response</span></span>

<span data-ttu-id="1bd17-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd17-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1bd17-174">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1bd17-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="1bd17-175">JSON</span><span class="sxs-lookup"><span data-stu-id="1bd17-175">JSON</span></span>

<span data-ttu-id="1bd17-176">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd17-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1bd17-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd17-177">Request</span></span>

<span data-ttu-id="1bd17-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bd17-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1bd17-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd17-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bd17-180">C#</span><span class="sxs-lookup"><span data-stu-id="1bd17-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bd17-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bd17-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bd17-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1bd17-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1bd17-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd17-183">Response</span></span>

<span data-ttu-id="1bd17-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd17-184">The following is an example of the response.</span></span>

> <span data-ttu-id="1bd17-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bd17-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
