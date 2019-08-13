---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Obtenha dados sobre as atividades do SharePoint por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8524636259e58833ec997602ecdfe4b7471eed2a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359884"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="9f5ed-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9f5ed-103">reportRoot: getSharePointActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f5ed-104">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="9f5ed-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="9f5ed-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f5ed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f5ed-106">Permissions</span></span>

<span data-ttu-id="9f5ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f5ed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f5ed-109">Permission type</span></span>                        | <span data-ttu-id="9f5ed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f5ed-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9f5ed-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f5ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f5ed-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f5ed-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9f5ed-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f5ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f5ed-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-114">Not supported.</span></span>                           |
| <span data-ttu-id="9f5ed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f5ed-115">Application</span></span>                            | <span data-ttu-id="9f5ed-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f5ed-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9f5ed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f5ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9f5ed-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9f5ed-118">Function parameters</span></span>

<span data-ttu-id="9f5ed-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9f5ed-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9f5ed-120">Parameter</span></span> | <span data-ttu-id="9f5ed-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f5ed-121">Type</span></span>   | <span data-ttu-id="9f5ed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f5ed-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9f5ed-123">ponto</span><span class="sxs-lookup"><span data-stu-id="9f5ed-123">period</span></span>    | <span data-ttu-id="9f5ed-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f5ed-124">string</span></span> | <span data-ttu-id="9f5ed-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9f5ed-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9f5ed-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9f5ed-128">data</span><span class="sxs-lookup"><span data-stu-id="9f5ed-128">date</span></span>      | <span data-ttu-id="9f5ed-129">Data</span><span class="sxs-lookup"><span data-stu-id="9f5ed-129">Date</span></span>   | <span data-ttu-id="9f5ed-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9f5ed-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9f5ed-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9f5ed-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9f5ed-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9f5ed-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-135">The default output type is text/csv.</span></span> <span data-ttu-id="9f5ed-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f5ed-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f5ed-137">Request headers</span></span>

| <span data-ttu-id="9f5ed-138">Nome</span><span class="sxs-lookup"><span data-stu-id="9f5ed-138">Name</span></span>          | <span data-ttu-id="9f5ed-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f5ed-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9f5ed-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f5ed-140">Authorization</span></span> | <span data-ttu-id="9f5ed-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9f5ed-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f5ed-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9f5ed-144">CSV</span><span class="sxs-lookup"><span data-stu-id="9f5ed-144">CSV</span></span>

<span data-ttu-id="9f5ed-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9f5ed-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9f5ed-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9f5ed-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9f5ed-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9f5ed-149">Report Refresh Date</span></span>
- <span data-ttu-id="9f5ed-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="9f5ed-150">User Principal Name</span></span>
- <span data-ttu-id="9f5ed-151">Excluído</span><span class="sxs-lookup"><span data-stu-id="9f5ed-151">Is Deleted</span></span>
- <span data-ttu-id="9f5ed-152">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="9f5ed-152">Deleted Date</span></span>
- <span data-ttu-id="9f5ed-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="9f5ed-153">Last Activity Date</span></span>
- <span data-ttu-id="9f5ed-154">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="9f5ed-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="9f5ed-155">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="9f5ed-155">Synced File Count</span></span>
- <span data-ttu-id="9f5ed-156">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="9f5ed-156">Shared Internally File Count</span></span>
- <span data-ttu-id="9f5ed-157">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="9f5ed-157">Shared Externally File Count</span></span>
- <span data-ttu-id="9f5ed-158">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="9f5ed-158">Visited Page Count</span></span>
- <span data-ttu-id="9f5ed-159">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="9f5ed-159">Assigned Products</span></span>
- <span data-ttu-id="9f5ed-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9f5ed-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9f5ed-161">JSON</span><span class="sxs-lookup"><span data-stu-id="9f5ed-161">JSON</span></span>

<span data-ttu-id="9f5ed-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-162">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9f5ed-163">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9f5ed-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f5ed-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9f5ed-165">CSV</span><span class="sxs-lookup"><span data-stu-id="9f5ed-165">CSV</span></span>

<span data-ttu-id="9f5ed-166">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9f5ed-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f5ed-167">Request</span></span>

<span data-ttu-id="9f5ed-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9f5ed-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f5ed-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f5ed-170">C#</span><span class="sxs-lookup"><span data-stu-id="9f5ed-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f5ed-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f5ed-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f5ed-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9f5ed-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f5ed-173">Java</span><span class="sxs-lookup"><span data-stu-id="9f5ed-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f5ed-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f5ed-174">Response</span></span>

<span data-ttu-id="9f5ed-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9f5ed-176">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="9f5ed-177">JSON</span><span class="sxs-lookup"><span data-stu-id="9f5ed-177">JSON</span></span>

<span data-ttu-id="9f5ed-178">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9f5ed-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f5ed-179">Request</span></span>

<span data-ttu-id="9f5ed-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9f5ed-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f5ed-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9f5ed-182">C#</span><span class="sxs-lookup"><span data-stu-id="9f5ed-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f5ed-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f5ed-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9f5ed-184">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9f5ed-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9f5ed-185">Java</span><span class="sxs-lookup"><span data-stu-id="9f5ed-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f5ed-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f5ed-186">Response</span></span>

<span data-ttu-id="9f5ed-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-187">The following is an example of the response.</span></span>

> <span data-ttu-id="9f5ed-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f5ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
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
